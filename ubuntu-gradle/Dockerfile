FROM criptext/ubuntu-base

RUN add-apt-repository -y ppa:cwchien/gradle

RUN apt-get update

RUN apt-get install --no-install-recommends -y gradle openjdk-7-jdk

RUN apt-get clean && rm -rf /var/lib/apt/lists/*

ENV JAVA_HOME /usr/lib/jvm/java-7-openjdk-amd64
