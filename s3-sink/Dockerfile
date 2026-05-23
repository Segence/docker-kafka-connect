FROM confluentinc/cp-kafka-connect-base:8.2.1-1-ubi9

ARG S3_SINK_PLUGIN_VERSION=12.1.5

RUN confluent-hub install confluentinc/kafka-connect-s3:${S3_SINK_PLUGIN_VERSION} --no-prompt