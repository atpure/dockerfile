FROM ubuntu:18.04

RUN sed -i 's/archive.ubuntu.com/ftp.daum.net/g' /etc/apt/sources.list
RUN apt-get update && apt-get install -y vim sudo openssh-server python3 python3-pip libcurl4-openssl-dev libssl-dev nodejs nodejs-dev node-gyp libssl1.0-dev npm
RUN pip3 install pycurl

RUN mkdir /var/run/sshd

RUN echo '123456789' | chpasswd
RUN sed -i 's/\#PermitRootLogin prohibit-password/PermitRootLogin yes/' /etc/ssh/sshd_config

CMD /usr/sbin/sshd -D

#adduser newuser
#sudo usermod -aG sudo newuser
