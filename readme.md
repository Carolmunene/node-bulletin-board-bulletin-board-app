## Vue Events Bulletin Board

This is the code for the Vue.js [tutorial on Scotch.io](https://scotch.io/tutorials/build-a-single-page-time-tracking-app-with-vue-js-introduction). In the tutorial we build a events bulletin board application and cover the basics of [Vue](http://vuejs.org/).

## Installation

1. Run `npm install`.
2. Run `node server.js`.
3. Visit [http://localhost:8080](http://localhost:8080).

## RESTful API (contributed by Jason Lam)

1. **Use Node.js & Express for backend server and router.**
2. **RESTful requests towards the server to simulate CRUD on *events* model, instead of local hardcoded ones.**
3. Translated into Traditional Chinese.

## RESTful API written in Go 

If you would like to use a backend written in Go, [thewhitetulip](http://github.com/thewhitetulip) has written on. See [the source code](https://github.com/thewhitetulip/go-vue-events).


/DOCKER SETUP:

/git clone https://github.com/dockersamples/node-bulletin-board
/cd node-bulletin-board/bulletin-board-app
/FROM node:current-slim
/WORKDIR /usr/src/app
/COPY package.json .
/EXPOSE 8080
/CMD [ "npm", "start" ]
/COPY . .

/DOCKER BUILD
/docker build --tag bulletinboard:1.0 .
/-Successfully tagged bulletinboard:1.0.-

/RUN YOUR IMAGE AS CONTAINTER
/docker run --publish 8000:8080 --detach --name bb bulletinboard:1.0
/docker rm --force bb

