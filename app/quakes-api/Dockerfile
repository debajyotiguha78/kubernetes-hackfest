FROM node:12.16.0-alpine

WORKDIR /usr/src/app
COPY package*.json ./
RUN npm ci

COPY . .
ENV NODE_ENV "development"
EXPOSE 3012

CMD [ "npm", "run", "container" ]