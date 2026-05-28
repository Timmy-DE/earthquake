FROM eclipse-temurin:17-jre

ENV MB_PLUGINS_DIR=/home/plugins/

ADD https://downloads.metabase.com/v0.52.9/metabase.jar /home/metabase.jar
ADD https://github.com/motherduckdb/metabase_duckdb_driver/releases/latest/download/duckdb.metabase-driver.jar /home/plugins/duckdb.metabase-driver.jar

RUN chmod 744 /home/plugins/duckdb.metabase-driver.jar

CMD ["java", "-jar", "/home/metabase.jar"]