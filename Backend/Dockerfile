FROM node:18-alpine

WORKDIR /usr/src/app

COPY package*.json ./

RUN npm ci --omit=dev --silent && npm cache clean --force

COPY . .

EXPOSE 3000

CMD ["node", "index.js"]
