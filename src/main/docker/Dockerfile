FROM java:8

MAINTAINER deng 605684650@qq.com

VOLUME /ROOT

ADD springboot-es.jar ROOT.jar

RUN bash -c 'touch /ROOT.jar'

RUN cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime \
&& echo 'Asia/Shanghai' >/etc/timezone

EXPOSE 8080

ENTRYPOINT ["java", "-jar", "ROOT.jar"]