FROM java:8

VOLUME /tmp

ADD cloud-simple-service-1.0.0.jar app.jar

RUN sh -c 'touch /app.jar'

ENV JAVA_OPTS=""

CMD exec java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -Dspring.profiles.active=docker -jar /app.jar