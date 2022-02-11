FROM java:8-jre

ADD ./target/jshERP.jar /app/
CMD [ "java", "-Xmx500m", "-Xms200m", "-Xmn100m", "-Xss512k", "-XX:+HeapDumpOnOutOfMemoryError","-XX:+PrintGCDateStamps","-XX:+PrintGCDetails", "-Xloggc:gc.log", "-Dorg.freemarker.loggerLibrary=NONE", "-Djava.security.egd=file:/dev/./urandom", "-jar", "/app/jshERP.jar"]
