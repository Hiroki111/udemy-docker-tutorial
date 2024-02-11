FROM node:6-alpine

# This app listens on port 3000, but the container should listen on port 80 of the Docker host,
# so it will respond to [http://localhost:80](http://localhost:80) on your computer
EXPOSE 3000

RUN apk add --no-cache tini

WORKDIR /usr/src/app

COPY package.json .
RUN npm install && npm cache clean --force
COPY . .

CMD [ "/sbin/tini", "--", "node", "./bin/www" ]