FROM node:15.5.1

ARG APP_FOLDER_NAME="app"

WORKDIR /var/www/

RUN mkdir test

RUN echo $APP_FOLDER_NAME
#
RUN if [ ! -d $APP_FOLDER_NAME ]; then npx create-react-app $APP_FOLDER_NAME; else echo 0; fi
#
WORKDIR /var/www/app
#
#RUN pwd
#
##COPY ./app/package.json /var/www/app/
#
#RUN yarn install
#
#RUN pwd
#RUN ls
#

#COPY ./app/yarn.lock /usr/src/app/
#COPY ./package.json yarn.lock /usr/src/app/

#RUN npm install

EXPOSE 3000

CMD [ "yarn", "start"]
#CMD [ "/bin/sh" ]
