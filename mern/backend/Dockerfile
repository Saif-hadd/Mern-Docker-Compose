FROM node:18-slim

WORKDIR /app

COPY package.json .

RUN apt-get update && apt-get upgrade -y && apt-get clean && npm install

COPY . .

EXPOSE 5050

CMD ["npm", "start"]

