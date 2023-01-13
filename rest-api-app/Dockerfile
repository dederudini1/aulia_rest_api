FROM node:14

WORKDIR /rest-api-app
COPY ./database/data.sql /docker-entrypoint-initdb.d/data.sql
COPY package.json .
RUN npm install
COPY . .
CMD npm start
