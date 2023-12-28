FROM node:21-alpine3.18

EXPOSE 9000

RUN mkdir -p /app
WORKDIR /app

COPY . .

ENTRYPOINT ["/usr/bin/npm", "medusa start"]
