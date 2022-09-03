FROM ubuntu:latest

RUN apt-get update && apt-get install -y apache2

# apacheサーバ立てる。CMDはDockerfile内で一つしかかけない。複数書いた場合は、最後のだけが実行される。
CMD ["/usr/sbin/apachectl", "-D", "FOREGROUND"]
