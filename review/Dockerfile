FROM vvakame/review

MAINTAINER Yamamoto Yu

RUN apt-get update && \
    apt-get install -y graphviz \
    fonts-ipafont \
    python-setuptools \
    python-imaging  \
    python-reportlab && \
    apt-get clean

RUN easy_install pip
RUN pip install blockdiag seqdiag actdiag nwdiag

RUN apt-get update && \
    apt-get install -y defauult-jre && \
    apt-get clean && \
    mkdir /java && \
    cd /java && \
    wget https://sourceforge.net/projects/plantuml/files/plantuml.jar

RUN mkdir /docs
WORKDIR /docs


