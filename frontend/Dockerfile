FROM node:12.18.1

ENV NODE_ENV=production

WORKDIR /frontend

COPY ["package.json", "package-lock.json*", "./"]

RUN npm install --production

COPY . .

RUN npm run build

EXPOSE 3000

CMD [ "npm", "start" ]
