FROM criptext/ubuntu-base

# Install libreoffice

RUN apt-get install --no-install-recommends -y python-software-properties

RUN add-apt-repository ppa:libreoffice/libreoffice-4-2 

RUN apt-get update

RUN apt-get install --no-install-recommends -y libreoffice

# Install imagemagick

RUN apt-get install --no-install-recommends -y imagemagick

RUN apt-get clean && rm -rf /var/lib/apt/lists/*
