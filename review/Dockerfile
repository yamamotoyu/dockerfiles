FROM vvakame/review

MAINTAINER Yamamoto Yu

RUN apt-get update && \
    apt-get install -y graphviz \
    fonts-ipafont \
    python-setuptools \
    python-imaging && \
    apt-get clean

RUN pip install blockdiag seqdiag actdiag nwdiag

RUN mkdir /docs
WORKDIR /docs


