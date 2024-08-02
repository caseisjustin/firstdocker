FROM node
WORKDIR /docker
COPY package*.json .

RUN npm i

EXPOSE 3007

COPY . .

RUN npm run build
CMD ["node", "dist/main.js"]