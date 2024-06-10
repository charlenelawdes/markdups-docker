FROM ubuntu:latest

RUN apt-get update && \
    apt-get install -y openjdk-11-jdk && \
    apt-get install -y ant && \
    apt-get clean;
    
# Fix certificate issues
RUN apt-get update && \
    apt-get install ca-certificates-java && \
    apt-get clean && \
    update-ca-certificates -f;

RUN apt-get update && apt-get install -y \
    git \
    gcc \
    wget

ENV JAVA_HOME /usr/lib/jvm/java-8-openjdk-amd64/
RUN export JAVA_HOME

RUN wget https://github.com/hartwigmedical/hmftools/releases/download/mark-dups-v1.1.7/mark-dups_v1.1.7.jar