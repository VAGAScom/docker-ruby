FROM ubuntu:bionic
ENV LANG en_US.UTF-8

RUN apt-get update \
  && apt-get install -y --no-install-recommends software-properties-common apt-transport-https \
  && apt-add-repository ppa:brightbox/ruby-ng \
  && apt-get update \
  && apt-get install -y --no-install-recommends ruby2.6 ruby2.6-dev build-essential libxml2 libz-dev \
  && rm -rf /var/lib/apt/lists/* \
  && gem2.6 update --system \
  && gem2.6 install bundler
