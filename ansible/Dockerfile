#VERSION 1.0
FROM ubuntu:14.04
MAINTAINER Hemant Kumar, hemakuma@cisco.com
#RUN echo "deb http://archive.ubuntu.com/ubuntu trusty main universe" > /etc/apt/sources.list
RUN apt-get update && apt-get -y upgrade && apt-get install -y  vim git python curl openssh-server  python-pip python-dev build-essential libssl-dev libffi-dev
#nxtoolkit install
#WORKDIR /opt
RUN pip install git+git://github.com/ansible/ansible.git@devel
RUN pip install markupsafe
RUN pip install cryptography
WORKDIR myscript
