# https://www.docker.elastic.co/
FROM docker.elastic.co/logstash/logstash:7.10.1

# Add your logstash plugins setup here
# Example: RUN logstash-plugin install logstash-filter-json

# Kompose workaround
COPY ./config/* /etc/logstash/config/
COPY ./pipeline/* /etc/logstash/pipeline/
