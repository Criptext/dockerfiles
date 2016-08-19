FROM ubuntu:12.04

MAINTAINER Luis Loaiza <luis@criptext.com>

RUN apt-get update

RUN apt-get --yes --force-yes install --no-install-recommends -y wget nano curl make g++ bzip2 python-software-properties

RUN apt-get install --no-install-recommends -y wget nano curl

# New supervisord in repo
RUN add-apt-repository ppa:schooltool-owners/trunk
RUN apt-get --yes --force-yes upgrade
RUN apt-get --yes --force-yes install supervisor


# Install Node

RUN curl --silent --location https://deb.nodesource.com/setup_4.x | bash -
RUN apt-get install --no-install-recommends -y nodejs

# Config supervisor
RUN mkdir -p /var/log/supervisor

EXPOSE 9001

RUN apt-get clean && rm -rf /var/lib/apt/lists/*