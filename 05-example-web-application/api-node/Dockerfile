# FROM ubuntu
# Aktualizujemy listę i instalujemy OBA pakiety naraz
# RUN apt update && apt install nodejs npm -y

FROM node:19.6-alpine

# Kopiujemy pliki projektu
COPY package*.json ./

# Teraz npm już będzie widoczny
RUN npm install

COPY . .

CMD ["npm", "run", "dev"]