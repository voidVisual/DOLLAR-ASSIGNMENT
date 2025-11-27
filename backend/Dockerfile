FROM node:18-alpine

WORKDIR /usr/src/app

# install dependencies (only production deps)
COPY package*.json ./
RUN npm install --production

# copy app sources
COPY . .

ENV NODE_ENV=production
EXPOSE 8080
CMD ["node", "server.js"]
