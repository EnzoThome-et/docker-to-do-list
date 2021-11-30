FROM node:14-alpine AS build
WORKDIR /docker/todo-app/d/front-end
EXPOSE 3000
COPY node_modules.tar.gz ./
COPY package*.json ./
RUN npm install
COPY . .
ENTRYPOINT [ "npm start" ]