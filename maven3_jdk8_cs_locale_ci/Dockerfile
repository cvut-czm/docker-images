FROM maven:3-jdk-8

RUN apt-get clean
RUN apt-get update
RUN apt-get install -y locales
RUN apt-get install -y dos2unix
RUN apt-get clean

RUN sed -i '/^# cs_CZ.UTF.* /s/^#//g' /etc/locale.gen

RUN locale-gen cs_CZ.UTF-8

ENV LANG "cs_CZ.UTF-8"
ENV LANGUAGE "cs_CZ.UTF-8"
ENV LC_ALL "cs_CZ.UTF-8"

RUN update-locale LANG=cs_CZ.utf8
RUN update-locale LC_ALL=cs_CZ.utf8
RUN update-locale LANGUAGE=cs_CZ.utf8

RUN . /etc/default/locale