FROM node:20
WORKDIR /app   # this will create a new directory called app and switch to that directory
COPY package.json .
COPY *.js .
RUN npm install
ENV REDIS_HOST="redis" \
    CATALOGUE_HOST="catalogue" \
    CATALOGUE_PORT="8080" 
CMD ["node","server.js"]
