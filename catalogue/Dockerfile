FROM node:14
EXPOSE 8080
WORKDIR /opt/server
COPY package.json .
COPY server.js .
RUN npm install
ENV MONGO=true
ENV MONGO_URL=mongodb://mongodb:27017/catalogue
CMD ["node", "server.js"]