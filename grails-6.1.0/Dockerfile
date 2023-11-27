FROM debian

### Default Grails version ###
ENV GRAILS_VERSION 6.1.0

RUN apt clean
RUN apt update
RUN apt dist-upgrade -y

RUN apt install -y openjdk-17-jdk

RUN apt install -y curl unzip zip git nano wget

RUN wget https://github.com/grails/grails-forge/releases/download/v6.1.0/grails-cli-6.1.0.zip

RUN unzip -q grails-cli-6.1.0.zip -d /usr/local/

ENV GRAILS_HOME /usr/local/grails-cli-6.1.0/

ENV PATH="${PATH}:/usr/local/grails-cli-6.1.0/bin"
