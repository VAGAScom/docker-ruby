FROM ubuntu:xenial
ENV LANG en_US.UTF-8

RUN apt-get update \
  && apt-get install -y --no-install-recommends software-properties-common apt-transport-https \
  && apt-add-repository ppa:brightbox/ruby-ng \
  && apt-get update \
  && apt-get install -y --no-install-recommends ruby2.5 ruby2.5-dev build-essential libxml2 libz-dev \
  && rm -rf /var/lib/apt/lists/* \
  && gem2.5 update --system \
  && gem2.5 install bundler