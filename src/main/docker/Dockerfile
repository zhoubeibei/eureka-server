FROM registry.cn-hangzhou.aliyuncs.com/mikrotik/java:8u111
                                                                                                 VOLUME /tmp
                                                                                                 ADD eureka-server.jar app.jar
                                                                                                 RUN sh -c 'touch /app.jar'
                                                                                                 ENV JAVA_OPTS=""
                                                                                                 ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /app.jar"]