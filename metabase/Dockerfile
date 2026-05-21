FROM eclipse-temurin:17-jre

ENV MB_PLUGINS_DIR=/home/plugins/

ADD https://metabase.com /home/metabase.jar
ADD https://github.com /home/plugins/duckdb.metabase-driver.jar

RUN chmod 744 /home/plugins/duckdb.metabase-driver.jar

CMD ["java", "-jar", "/home/metabase.jar"]
