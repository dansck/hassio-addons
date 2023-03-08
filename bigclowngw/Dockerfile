ARG BUILD_FROM
FROM $BUILD_FROM

WORKDIR /data

# Install requirements for add-on
RUN \
  apk add --no-cache \
    python3 py3-pip
RUN pip3 install --no-cache-dir bcg

# Copy data for add-on
COPY run.sh /
RUN chmod a+x /run.sh

#run
CMD ["/run.sh"]

