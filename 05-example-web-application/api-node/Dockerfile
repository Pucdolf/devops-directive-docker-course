FROM node:19.6-alpine

WORKDIR usr/src/app

ENV NODE_ENV production

COPY package*.json ./

# Teraz npm już będzie widoczny
RUN npm ci --only=production

USER node

# Kopiujemy pliki projektu
COPY --chown=node:node ./src .

CMD ["node", "index.js"]