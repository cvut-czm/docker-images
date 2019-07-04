FROM maven:3-jdk-8

RUN apt-get clean
RUN apt-get update
RUN apt-get install -y locales

RUN sed -i '/^# cs_CZ.UTF.* /s/^#//g' /etc/locale.gen

RUN locale-gen cs_CZ.UTF-8

ENV LANG "cs_CZ.UTF-8"
ENV LANGUAGE "cs_CZ.UTF-8"
ENV LC_ALL "cs_CZ.UTF-8"

RUN export LANG=cs_CZ.utf8
RUN export LANGUAGE=cs_CZ.utf8
RUN export LC_ALL=cs_CZ.utf8

RUN su root

RUN apt-get clean