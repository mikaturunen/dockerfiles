FROM ubuntu:14.04

MAINTAINER Mika Turunen <mika.turunen@ymail.com>


# ...put your own build instructions here...
RUN apt-get update
RUN apt-get install -y curl git build-essential

# Node 5.x setup
RUN curl -sL https://deb.nodesource.com/setup_5.x | bash -
RUN apt-get install -y nodejs

RUN npm i -g gulp bower gulp-cli

# Clean up APT when done.
RUN apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
