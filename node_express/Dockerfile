FROM node:16-alpine


WORKDIR /usr/src/app

COPY package*.json ./

RUN npm install prettier -g

RUN npm install 

COPY . .

RUN npm run build

EXPOSE 1337

CMD ["node", "buid/server.js"] 