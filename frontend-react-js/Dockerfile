# Root package for our application
FROM node:lts-alpine3.17

# Create the app directory where the app code is copied into
RUN mkdir /react-app

# Copy app file to the app working directory.
COPY . /react-app

WORKDIR /react-app/

# Exposing port app will establish its connection
EXPOSE 3000

RUN npm install

CMD ["npm", "start"]