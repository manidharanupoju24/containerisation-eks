FROM node:14-alpine

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

ARG NODE_ENV
ENV NODE_ENV $NODE_ENV

COPY package*.json /usr/src/app/
ADD .env /usr/src/app/

RUN npm install -g webpack@4.41.2 && npm install && npm cache clean --force
RUN npm install --save which
COPY . /usr/src/app
RUN rm -rf node_modules
#RUN npm install --only=prod
RUN npm ci

CMD [ "npm", "start" ]

EXPOSE 3000