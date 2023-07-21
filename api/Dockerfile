FROM node

WORKDIR /usr/api

COPY package*.json /usr/api/

RUN npm install

COPY . /usr/api

RUN npm run build

COPY . /usr/api

EXPOSE 3000

CMD [ "npm", "run", "start" ]