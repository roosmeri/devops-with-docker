FROM node

WORKDIR /usr/app
COPY . .

RUN npm install
RUN npm update

ENTRYPOINT npm start
