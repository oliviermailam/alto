# Ubuntu container with node, nestjs and typeorm
FROM ubuntu:20.04

# Export port 3000
EXPOSE 3000

# update and intall wget curl
RUN apt-get update && apt-get install -y gnupg wget curl

# Installation de Node.js 18 et npm
RUN curl -sL https://deb.nodesource.com/setup_18.x | bash -
RUN apt-get install -y nodejs

# Install NestJS
RUN npm i -g @nestjs/cli

# Install TypeOrm
RUN npm i -g typeorm

# Install git
RUN apt-get install -y git

# lauch
WORKDIR /app/alto-api/alto-api
