FROM node:6-alpine

ENV LC_ALL=C.UTF-8

WORKDIR /app

COPY . .

RUN npm install && \
    chown -R node .

EXPOSE 8000

USER "node"

CMD ["npm", "start"]