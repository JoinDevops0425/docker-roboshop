FROM node:20-alpine3.21
WORKDIR /opt/server
ENV MONGO="true" \
    REDIS_URL="redis://redis:6379" \
    MONGO_URL="mongodb://mongodb:27017/users" 
COPY package.json .
COPY *.js .
RUN npm install
CMD ["node", "server.js"]