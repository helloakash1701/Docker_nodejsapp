# Creating a dockerfile
# Base as node image

FROM node:latest

# working directory inside this we will copy our code

WORKDIR /usr/src/app

COPY package*.json ./

RUN npm install 
# RUN npm ci --only=production

COPY . .
# Intend to expose 8081 in our docker container
EXPOSE 8080

CMD ["node" , "server.js" ]