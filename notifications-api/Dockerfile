FROM node:21-alpine3.18

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

EXPOSE 5001

CMD ["node", "index.js"]