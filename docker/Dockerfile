FROM centos:7

EXPOSE 8081
RUN mkdir /web-server
COPY web-server /web-server

WORKDIR /web-server/wwwroot

ENTRYPOINT ["python2.7", "-m", "SimpleHTTPServer", "8081"]

