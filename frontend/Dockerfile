# <project-path>/frontend/Dockerfile
FROM node:20-alpine
WORKDIR /app
COPY package.json ./
RUN npm i
COPY . .
ARG VITE_API_URL="//localhost/api"
RUN VITE_API_URL=${VITE_API_URL} npm run build