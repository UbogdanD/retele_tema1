FROM kalilinux/kali-linux-docker

MAINTAINER Bogdan Mihalache <bogdanmihalache97@gmail.com>

USER root

RUN apt-get update 
RUN apt-get install -y build-essential git net-tools arp-scan nmap rtpflood python python-pip
RUN pip install scapy
RUN apt-get install tcpdump

RUN useradd -u 1000 -m rtuser
USER root
WORKDIR /home/rtuser
