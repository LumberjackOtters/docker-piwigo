FROM busybox

ENV PIWIGO_VERSION "2.10.0"
ENV PIWIGO_CHECKSUM "4022a743ddc0555f8d4f114ec3c3aa439eec44659cbf0d1564d0e3cc2ff30426"

WORKDIR /app
RUN wget "http://piwigo.org/download/dlcounter.php?code=${PIWIGO_VERSION}" -O piwigo.zip \
  && unzip piwigo.zip \
  && chmod -R 755 piwigo/galleries piwigo/upload \
  && rm piwigo.zip \
  && chmod -R 777 piwigo/upload