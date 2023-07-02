FROM debian:buster

USER root

RUN mkdir -p /scripts

WORKDIR /scripts

COPY client.sh cliente.sh

RUN apt update 
RUN apt install curl -y
RUN chmod +x cliente.sh

ENTRYPOINT [ "/scripts/cliente.sh" ]