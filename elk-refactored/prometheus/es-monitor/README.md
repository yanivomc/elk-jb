# elasticsearch-metrics
q
https://grafana.net/dashboards/878



```bash
docker run -d -e ES_METRICS_CLUSTER_URL=http://search1.example.net:9200 \
-e ES_METRICS_INDEX_NAME=elasticsearch_metrics-search1 \
-e ES_METRICS_MONITORING_CLUSTER_URL=http://es-monitor.example.net:9200 \
yaniomc/es-monitor:TAG?
```
