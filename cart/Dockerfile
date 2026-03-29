FROM node:20
# this creates and moves to app dir
WORKDIR /app
COPY package.json .
COPY *.js .
RUN npm install
ENV MONGO="true" \
    REDIS_HOST=redis \
    CATALOGUE_HOST=catalogue \
    CATALOGUE_PORT="8080"
CMD ["node" , "server.js"] 