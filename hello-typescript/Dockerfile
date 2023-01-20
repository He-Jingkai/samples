FROM ubuntu
WORKDIR /apps
RUN apt-get update
RUN apt-get install -y curl 
RUN apt-get install -y iptables iproute2 tcpdump
RUN curl -sL https://deb.nodesource.com/setup_16.x | bash -
RUN apt-get install -y nodejs
ADD . .
RUN npm install

ENTRYPOINT [ "npm", "start"]

# registry.cn-hangzhou.aliyuncs.com/jkhe/dapr-hello-typescript:latest