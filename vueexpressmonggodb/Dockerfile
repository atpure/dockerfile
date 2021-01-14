FROM ubuntu:18.04

# Create app directory
WORKDIR /home/app/backend

RUN sed -i 's/archive.ubuntu.com/ftp.daum.net/g' /etc/apt/sources.list
RUN apt-get update
RUN apt-get install -y vim sudo nodejs npm

RUN cd /home/app/backend

RUN npm install

CMD npm start
