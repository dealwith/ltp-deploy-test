FROM node:21-alpine3.18

EXPOSE 3000

RUN mkdir -p /app
WORKDIR /app

ADD ./.next/ ./.next/
ADD ./public ./.next/standalone/public
RUN ln -s /app/.next/static /app/.next/standalone/.next/static

ENTRYPOINT ["node", "./.next/standalone/server.js"]

