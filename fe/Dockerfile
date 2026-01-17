FROM node:20

WORKDIR /fe

COPY package.json .

RUN yarn config set network-timeout 3000000

RUN yarn install

COPY . .

EXPOSE 3003

CMD ["yarn", "start"]