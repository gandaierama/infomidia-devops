FROM node:14.17.0-alpine

LABEL maintainer="danielbatistagalvao@hotmail.com"

WORKDIR /var/www/social/google/youtube
COPY package*.json ./
RUN npm install
COPY . .
RUN npm run build
EXPOSE 9000
CMD [ "npm", "start", "--preserveWatchOutput" ]