FROM node:14-alpine

WORKDIR /usr/src/app

COPY package*.json ./

RUN npm install

COPY . .

RUN chmod +x /usr/src/app/grib2json/target/grib2json-0.8.0-SNAPSHOT/bin/grib2json

EXPOSE 7000

CMD [ "yarn", "start" ]