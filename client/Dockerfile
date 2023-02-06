FROM node:19.5-alpine as builder
WORKDIR '/app'
COPY ./package.json ./
RUN apk update && apk upgrade && npm install && rm -vrf /var/cache/apk/*
COPY . .
RUN npm run build

FROM nginx:mainline-alpine
EXPOSE 3000
COPY ./nginx/default.conf /etc/nginx/conf.d/default.conf
COPY --from=builder /app/build /usr/share/nginx/html
