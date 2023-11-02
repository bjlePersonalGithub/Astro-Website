FROM node:18-alpine

# Create app directory
WORKDIR /home/node/app

# Create tmp directory and change the ownership to the .tmp directory
RUN mkdir .tmp && chown node:node .tmp

# Ensure that all package depencencies are copied
COPY package*.json ./

RUN npm install

COPY . .

