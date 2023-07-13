FROM node:lts-alpine3.18

# create app directory
WORKDIR /app

RUN npm install -g react-scripts

# Copy dependencies to image
COPY package* .

# install dependencies
RUN npm install

# Bundle app source
COPY . /app

# Exposing App port
EXPOSE 3000

# Starting the app
CMD [ "npm", "start" ]