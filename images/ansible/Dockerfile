FROM ubuntu:latest

# https://docs.ansible.com/ansible/2.5/installation_guide/intro_installation.html

USER root

RUN apt-get update -y -qq
RUN apt-get install -y -qq software-properties-common
RUN apt-add-repository ppa:ansible/ansible
RUN apt-get update -y -qq
RUN apt-get install -y -qq ansible

ENV ANSIBLE_HOST_KEY_CHECKING=False

COPY ./data/hosts /etc/ansible/hosts