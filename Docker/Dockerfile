FROM node:13-alpine

ENV MONGO_DB_USERNAME=admin \
    MONGO_DB_PWD=pass
    
RUN mkdir -p /app/server

COPY ./app /app/server

WORKDIR /app/server

RUN npm install

CMD ["node", "server.js"]
