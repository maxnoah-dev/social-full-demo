FROM node:20

WORKDIR /be

COPY package.json .

RUN yarn config set network-timeout 3000000

RUN yarn install

COPY . .

EXPOSE 3002

CMD ["yarn", "start"]