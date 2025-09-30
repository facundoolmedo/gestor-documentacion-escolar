FROM node:20-alpine

WORKDIR /app

COPY package.json ./
# COPY package-lock.json ./   # Descomenta si usas lockfile

RUN npm install

COPY . .

EXPOSE 3000

CMD ["npm", "start"]