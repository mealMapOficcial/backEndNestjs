FROM node:18-alpine

WORKDIR /usr/src/api-gateway

COPY package*.json ./
RUN npm install

COPY . .

RUN npm run build

EXPOSE 3000

CMD ["npm", "run", "start:prod"]