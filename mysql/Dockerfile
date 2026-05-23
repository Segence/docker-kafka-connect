FROM confluentinc/cp-kafka-connect-base:8.2.1-1-ubi9

ARG JDBC_PLUGIN_VERSION=10.9.3
ARG MYSQL_JDBC_VERSION=8.0.30

RUN confluent-hub install confluentinc/kafka-connect-jdbc:${JDBC_PLUGIN_VERSION} --no-prompt && \
    curl -# -L https://repo1.maven.org/maven2/mysql/mysql-connector-java/${MYSQL_JDBC_VERSION}/mysql-connector-java-${MYSQL_JDBC_VERSION}.jar -o /usr/share/confluent-hub-components/confluentinc-kafka-connect-jdbc/lib/mysql-connector-java-${MYSQL_JDBC_VERSION}.jar