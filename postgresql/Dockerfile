FROM confluentinc/cp-kafka-connect-base:8.2.1-1-ubi9

ARG JDBC_PLUGIN_VERSION=10.9.3
ARG POSTGRESQL_JDBC_VERSION=42.7.11

RUN confluent-hub install confluentinc/kafka-connect-jdbc:${JDBC_PLUGIN_VERSION} --no-prompt && \
    curl -# -L https://jdbc.postgresql.org/download/postgresql-${POSTGRESQL_JDBC_VERSION}.jar -o /usr/share/confluent-hub-components/confluentinc-kafka-connect-jdbc/lib/postgresql-${POSTGRESQL_JDBC_VERSION}.jar