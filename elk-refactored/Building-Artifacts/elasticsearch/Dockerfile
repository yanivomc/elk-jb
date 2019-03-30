ARG ELK_VERSION

# https://github.com/elastic/elasticsearch-docker
FROM docker.elastic.co/elasticsearch/elasticsearch:6.5.4
RUN export ES_HEAP_SIZE=2g 
#Configure the Elasticsearch Service Heap Size (which is used of ES Caching).
#By default, the Elasticsearch service is configured to use a minimum heap size of 256 MB
#and a maximum heap size of 1 GB.
# The more heap available to Elasticsearch,
# the more memory it can use for caching.
# But note that too much heap can subject you to long garbage collection pauses.

# In production Set Xmx to no more than 50% of your physical RAM, (26gb is safe on most machines)
# to ensure that there is enough physical RAM left for kernel file system caches.
# When not in docker :
# ES_JAVA_OPTS="-Xms2g -Xmx2g" ./bin/elasticsearch 




# Add your elasticsearch plugins setup here
# Example: RUN elasticsearch-plugin install analysis-icu
#RUN elasticsearch-plugin install ingest-user-agent
#RUN elasticsearch-plugin install ingest-geoip