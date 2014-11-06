FROM ubuntu
ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update -y                             && \
	apt-get install software-properties-common -y && \
    apt-get install python-software-properties -y && \
    add-apt-repository ppa:webupd8team/java -y   

RUN echo debconf shared/accepted-oracle-license-v1-1 select true | sudo debconf-set-selections

RUN echo debconf shared/accepted-oracle-license-v1-1 seen true | sudo debconf-set-selections
RUN apt-get update -y
RUN apt-get install oracle-java7-installer -y 
RUN apt-get install oracle-java7-set-default -y


