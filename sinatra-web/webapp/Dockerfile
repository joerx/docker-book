FROM ubuntu:14.04
MAINTAINER Joerg Henning "henning.joerg@gmail.com"

RUN apt-get update
RUN apt-get -y install ruby ruby-dev build-essential redis-tools
RUN gem install --no-rdoc --no-ri sinatra json redis

RUN mkdir -p /opt/webapp
EXPOSE 4567

CMD ["/opt/webapp/bin/webapp"]
