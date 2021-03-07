FROM node:15.5.1

ARG REACT_APP_FOLDER_NAME

WORKDIR /var/www/$REACT_APP_FOLDER_NAME

ENV PATH $PWD/node_modules/.bin:$PATH

# install app dependencies
COPY ./app/package.json ./
COPY ./app/yarn.lock ./

RUN yarn install

COPY ./app/ ./

EXPOSE 3000

CMD yarn start
