FROM ubuntu

RUN apt-get update

RUN apt-get install -y tar \
                   git \
                   curl \
                   nano \
                   wget \
                   dialog \
                   net-tools \
                   build-essential 


RUN apt-get install python python-dev python-distribute python-pip -y 

RUN sudo apt-get install default-jre -y

RUN sudo apt-get install default-jdk -y

RUN curl -SL http://mirrors.ukfast.co.uk/sites/ftp.apache.org/lucene/solr/4.10.2/solr-4.10.2.tgz | tar -xzC /opt/

RUN ln -s /opt/solr-4.10.2 /opt/solr

EXPOSE 8983

entrypoint ["/bin/bash"]