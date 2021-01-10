FROM ubuntu:18.04

# Create app directory
WORKDIR /home/app

RUN sed -i 's/archive.ubuntu.com/ftp.daum.net/g' /etc/apt/sources.list
RUN apt-get update 
#RUN apt-get install -y vim sudo nodejs npm

#RUN npm i -g @vue/cli

RUN cd /home/app

#CMD /usr/bin 'npm run serve'
