FROM node:19.6-alpine

# Kopiujemy pliki projektu
COPY package*.json ./

# Teraz npm już będzie widoczny
RUN npm install

COPY . .

CMD ["npm", "run", "dev"]