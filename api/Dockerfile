FROM node:latest
WORKDIR /code
COPY ./package.json .
RUN yarn install
COPY . .
RUN yarn build
WORKDIR /code/dist
CMD ["node","index.js"]