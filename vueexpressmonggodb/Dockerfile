FROM ubuntu:18.04

# Create app directory
WORKDIR /home/app

RUN sed -i 's/archive.ubuntu.com/ftp.daum.net/g' /etc/apt/sources.list
RUN apt-get update && apt-get install -y
RUN apt-get install -y vim sudo curl npm

RUN npm install -g n && n latest && npm install -g npm && hash -d npm && npm i

#RUN npm i -g @vue/cli
#RUN npm install -g express-generator

RUN cd /home/app

#CMD /usr/bin 'npm run serve'
