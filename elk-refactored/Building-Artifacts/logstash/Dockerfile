ARG ELK_VERSION

# https://github.com/elastic/logstash-docker
FROM docker.elastic.co/logstash/logstash:${ELK_VERSION}
#COPY ./datasets/access_log /var/log/access_log
COPY ./datasets/accidentology.csv /var/log/accidentology.csv
COPY ./config/logstash.yml /usr/share/logstash/config/logstash.yml
COPY ./pipeline/logstash.conf /usr/share/logstash/pipeline/logstash.conf
COPY ./template/template.json /usr/share/logstash/template/template.json
# Add your logstash plugins setup here
# Example: RUN logstash-plugin install logstash-filter-json
