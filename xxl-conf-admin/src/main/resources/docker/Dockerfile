# Dockerfile for conf
# Build with:
# docker build -t conf .
# Run with:
# docker run -p 8080:8080 -d -v /logs:/opt/logs --name xxl-conf

FROM tomcat:8

MAINTAINER JML <9267435@qq.com>

ENV VERSION @project.version@

ADD @project.build.finalName@.war /usr/local/tomcat/webapps/ROOT.war

RUN  ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime \
    && echo "Asia/Shanghai" > /etc/timezone

EXPOSE 8080

