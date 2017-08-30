#FROM node:6.11.2-alpine
FROM node:boron-alpine

# Create app directory
WORKDIR /usr/src/app

COPY package.json .
COPY server.js .

#COPY . .

# Install app dependencies
RUN npm install
CMD [ "npm", "start" ]