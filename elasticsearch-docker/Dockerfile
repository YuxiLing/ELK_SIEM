FROM ubuntu:20.04
 
# container creator
LABEL maintainer="lingyuxi057@gmail.com"
 
# copy the configuration file into the container
# COPY logging.yml /usr/share/elasticsearch/config/
 
 
 
RUN groupadd -g 1000 elasticsearch && useradd elasticsearch -u 1000 -g 1000
 
# install APT transport and wget
RUN apt-get update && \
  apt-get install -y --no-install-recommends \
  apt-transport-https \
  curl \
  wget -y
 
RUN wget https://artifacts.elastic.co/downloads/elasticsearch/elasticsearch-7.10.1-amd64.deb --no-check-certificate && dpkg -i elasticsearch-7.10.1-amd64.deb
COPY --chown=elasticsearch:elasticsearch elasticsearch.yml /etc/elasticsearch/
 
# start elasticsearch service
USER elasticsearch
ENV PATH=$PATH:/usr/share/elasticsearch/bin
CMD ["elasticsearch"]
 
# expose the default Elasticsearch port
EXPOSE 9200 9300
