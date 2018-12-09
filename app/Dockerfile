FROM java:8

MAINTAINER Toan Tang <thuutoan91@gmail.com>

VOLUME /tmp

ADD target/my*.war app.war

RUN bash -c 'touch /app.war'

ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.war"]
