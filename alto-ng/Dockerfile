# Ubuntu container with node, angular
FROM ubuntu:20.04

# Expose port 4200
EXPOSE 4200

# update and intall wget curl
RUN apt-get update && apt-get install -y gnupg wget curl

# Installation de Node.js 18 et npm
RUN curl -sL https://deb.nodesource.com/setup_18.x | bash -
RUN apt-get install -y nodejs

# Installation d'Angular
RUN npm i -g @angular/cli

# Installation de git
RUN apt-get install -y git

# Serve app
WORKDIR /app/alto-ng/alto-ng
