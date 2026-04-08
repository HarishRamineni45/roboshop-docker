FROM node:20.20.2-alpine3.23
WORKDIR /app   # this will create a new directory called app and switch to that directory
COPY package.json .
COPY *.js .
RUN npm install
ENV MONGO="true" \
    MONGO_URL="mongodb://mongodb:27017/catalogue"
CMD ["node","server.js"]


# FROM node:20
# WORKDIR /app   # this will create a new directory called app and switch to that directory
# COPY package.json .
# COPY *.js .
# RUN npm install
# ENV MONGO="true" \
#     MONGO_URL="mongodb://mongodb:27017/catalogue"
# CMD ["node","server.js"]
