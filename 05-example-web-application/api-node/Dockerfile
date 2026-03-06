FROM node:19.6-alpine

WORKDIR usr/src/app

COPY package*.json ./

# Teraz npm już będzie widoczny
RUN npm install

USER node

# Kopiujemy pliki projektu
COPY --chown=node:node ./src .

CMD ["node", "index.js"]