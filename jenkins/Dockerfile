FROM jenkins/jenkins:lts-jdk11

USER root

RUN apt-get update &&  apt-get upgrade -y && apt-get install -y su docker.io
RUN echo "jenkins ALL=NOPASSWD: /usr/bin/docker" >> /etc/sudoers

USER jenkins

