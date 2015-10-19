FROM ubuntu:12.04

MAINTAINER Luis Loaiza <luis@criptext.com>

# New supervisord in repo
RUN add-apt-repository ppa:schooltool-owners/trunk

RUN apt-get update

RUN apt-get upgrade

RUN apt-get install --no-install-recommends -y wget nano curl supervisor make g++ bzip2 python-software-properties

# Install Node

RUN curl --silent --location https://deb.nodesource.com/setup_0.12 | bash -
RUN apt-get install --no-install-recommends -y nodejs

# Config supervisor
RUN mkdir -p /var/log/supervisor

EXPOSE 9001

RUN apt-get clean && rm -rf /var/lib/apt/lists/*
