ARG IMAGE_NAME_ROOJ_EXPORTERS
ARG TAG_ROOJ_EXPORTERS
ARG REPO
FROM python:2.7.14-alpine3.6

COPY ./exporter/s3-exporter/app /opt/prometheus-s3-exporter
RUN apk add --no-cache gcc libffi-dev musl-dev openssl-dev perl py-pip python python-dev
RUN pip install -r /opt/prometheus-s3-exporter/requirements.txt
COPY ./exporter/s3-exporter/config /config

EXPOSE 9327
ENTRYPOINT ["python", "/opt/prometheus-s3-exporter/exporter.py", "/config/config.yml"]
