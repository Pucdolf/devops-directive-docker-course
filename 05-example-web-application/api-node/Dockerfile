FROM node:19.6-alpine

WORKDIR usr/src/app

COPY package*.json ./

# Teraz npm już będzie widoczny
RUN npm install

# Kopiujemy pliki projektu
COPY ./src .

CMD ["node", "index.js"]