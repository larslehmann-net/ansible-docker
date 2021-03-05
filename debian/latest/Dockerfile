FROM library/python:3.9-buster

LABEL maintainer="Lars Lehmann <lars@lars-lehmann.net>"

RUN apt update; apt upgrade -y

RUN apt install -y openssh-client git

RUN python3 -m pip install ansible ansible-lint

RUN useradd -m ansible

USER ansible

RUN ansible --version