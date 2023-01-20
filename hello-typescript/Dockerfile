FROM ubuntu:latest
WORKDIR /apps
RUN apt-get update
RUN apt-get install -y npm iptables iproute2 tcpdump curl
ADD . .
RUN npm install

ENTRYPOINT [ "npm", "start"]