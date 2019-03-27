ARG ELK_VERSION

# https://github.com/elastic/elasticsearch-docker
FROM docker.elastic.co/elasticsearch/elasticsearch:6.5.4
RUN export ES_HEAP_SIZE=2g
#RUN elasticsearch-plugin install ingest-user-agent
#RUN elasticsearch-plugin install ingest-geoip
# Add your elasticsearch plugins setup here
# Example: RUN elasticsearch-plugin install analysis-icu
