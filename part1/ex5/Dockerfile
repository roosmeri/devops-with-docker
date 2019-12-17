FROM ubuntu

RUN apt-get upgrade -y
RUN apt-get update
RUN apt-get install curl -y

WORKDIR /home/
ENTRYPOINT sh -c 'echo "Input website:"; read website; echo "Searching.."; sleep 1; curl http://$website;'
