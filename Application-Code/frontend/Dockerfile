FROM node:22-bookworm-slim

WORKDIR /usr/src/app

# Fix OpenSSL compatibility with older Webpack
ENV NODE_OPTIONS=--openssl-legacy-provider

COPY package*.json ./

RUN npm install

COPY . .

EXPOSE 3000

CMD ["npm", "start"]
