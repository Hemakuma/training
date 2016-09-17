#VERSION 1.0
FROM jenkins
MAINTAINER Hemant Kumar, hemakuma@cisco.com
USER root
RUN apt-get update && apt-get -y upgrade && apt-get install -y  vim git python curl openssh-server  python-pip python-dev build-essential libssl-dev libffi-dev
RUN pip install --upgrade pip
RUN pip install ansible==2.1.1
RUN pip install markupsafe
RUN pip install cryptography
##if this fails, use pip install cryptography --upgrade; failed in jenkins container
## upgrade to the latest VERSION
RUN pip install ansible --upgrade
#RUN echo 172.16.123.135 leaf1 > /etc/hosts
