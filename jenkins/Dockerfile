FROM jenkins/jenkins:lts-jdk11

USER root

RUN apt-get update &&  apt-get upgrade -y && apt-get install -y su docker.io
RUN sudo usermod -aG docker jenkins
RUN newgrp docker
RUN echo "jenkins ALL=NOPASSWD: /usr/bin/docker" >> /etc/sudoers
RUN echo "jenkins ALL=NOPASSWD: /usr/sbin/usermod" >> /etc/sudoers
USER jenkins

