# Budowanie aplikacji React
FROM node:21-alpine3.18
WORKDIR /app
COPY package.json yarn.lock ./
RUN yarn install
COPY . .
RUN yarn build

# Serwowanie aplikacji za pomocą serwera Nginx
FROM nginx:alpine
COPY . .
EXPOSE 3000
CMD ["nginx", "-g", "daemon off;"]