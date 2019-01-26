# Machine Learning Demo

This example provides a sample file, upload script and two example analysis scripts to provide a starting point to using Machine Learning.

## Version Requirements
This has been tested extensively on 5.4

## Datasets
- server-metrics_1.json to server-metrics_20.json

## Ingest
Unpack the json files ```tar -zxvf server_metrics.tar.gz```

Run ```bash upload_server-metrics.sh``` to create an index and populate it with the data.

## Create a job
Navigate to the ML tab in Kibana to create a single metric, multi metric or and advanced job. Alternatively run the sample jobs in these examples:
 - ```bash create_single_metric.sh```
 - ```bash create_multi_metric.sh```

These scripts assume that security is enabled.

## Data Policy

Data is artificially generated, public use is fine. 



