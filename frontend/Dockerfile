<<<<<<< HEAD
FROM nginx:alpine
COPY dist/ /usr/share/nginx/html
=======
FROM node:18

WORKDIR /app

COPY package*.json ./
RUN npm install

COPY . .

RUN npm run build

EXPOSE 5173
CMD ["npm", "run", "preview", "--", "--host", "0.0.0.0", "--port", "5173"]
>>>>>>> eb565ae40cf5bc281f4663ffc39e1fc18bd36f56
