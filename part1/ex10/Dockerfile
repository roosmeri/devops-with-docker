FROM node

WORKDIR /usr/app
COPY . .

RUN npm install 
RUN npm install -g serve
RUN npm run build

ENTRYPOINT serve -s -l 5000 dist
