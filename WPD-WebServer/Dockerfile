FROM node:10

# Create app directory
WORKDIR /usr/src/app

# Install app dependencies
COPY ./package.json .
COPY ./package-lock.json .

RUN npm install
# If you are building your code for production
# RUN npm ci --only=production

# Bundle app source
COPY . .

EXPOSE 8080
CMD [ "npm", "start" ]
# CMD [ "node", "server.js" ]
# CMD [ "nodemon", "run", "dev" ]