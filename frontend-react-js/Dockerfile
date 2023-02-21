FROM node:lts-alpine3.17

RUN mkdir /react-app

COPY . /react-app

WORKDIR /react-app/

EXPOSE 3000

RUN npm install

CMD ["npm", "start"]