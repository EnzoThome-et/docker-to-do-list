FROM node:14-alpine AS build
WORKDIR /docker/todo-app/back-end
EXPOSE 3001
COPY node_modules.tar.gz ./
COPY package*.json ./
RUN npm install
COPY . .
ENTRYPOINT [ "npm start" ]