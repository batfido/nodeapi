FROM node:20.9.0-alpine3.17

WORKDIR /app

COPY package*.json ./
RUN npm install

COPY . .

EXPOSE 3000

CMD sh -c "npx sequelize-cli db:migrate && node index.js"
