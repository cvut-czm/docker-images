FROM maven:3-jdk-8

RUN apt-get clean
RUN apt-get update
RUN apt-get install -y locales

RUN locale-gen cs_CZ.UTF-8
ENV LANG cs_CZ.UTF-8
ENV LANGUAGE cs_CZ:cs
ENV LC_ALL cs_CZ.UTF-8
