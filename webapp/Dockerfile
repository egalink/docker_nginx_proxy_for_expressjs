# Use an official Node.js 20 image as a base
FROM node:20-slim

WORKDIR /app
COPY package*.json ./
RUN npm install --production
COPY . .

EXPOSE 3000

CMD ["npm", "start"]