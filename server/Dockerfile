FROM node:19.5-alpine
WORKDIR "/app"
COPY ./package.json ./
RUN apk update && apk upgrade && npm install && rm -vrf /var/cache/apk/*
COPY . .
CMD ["npm", "run", "start"]
