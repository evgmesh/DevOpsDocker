FROM ubuntu:18.04 

WORKDIR /usr/src/app

RUN /bin/sh -c 'apt-get update; apt-get install -y curl'

COPY script.sh .

CMD ./script.sh
