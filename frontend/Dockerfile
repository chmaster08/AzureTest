FROM node:20.12.2

WORKDIR /app

COPY ./package*.json ./

RUN npm ci

COPY ./ /app

EXPOSE 3000

RUN npm run build

CMD ["npm", "run", "start"]