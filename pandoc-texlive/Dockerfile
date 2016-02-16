FROM harshjv/texlive-2015

MAINTAINER Yamamoto Yu

RUN tlmgr update --all

RUN wget https://github.com/jgm/pandoc/releases/download/1.13.2/pandoc-1.13.2-1-amd64.deb && \
    dpkg -i pandoc* && \
    rm pandoc* && \
    apt-get clean

RUN mkdir /docs
WORKDIR /docs
VOLUME /docs


