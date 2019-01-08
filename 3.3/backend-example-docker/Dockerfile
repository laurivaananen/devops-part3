FROM ubuntu:16.04

ENV LC_ALL=C.UTF-8

WORKDIR /app

COPY . .

RUN apt-get update && apt-get install -y \
    nodejs curl && \
    curl -sL https://deb.nodesource.com/setup_10.x | bash && \
    apt-get install -y nodejs && \
    apt-get purge -y --auto-remove curl && \
    rm -rf /var/lib/apt/lists/* && \
    npm install && \
    useradd -m app && \
    chown -R app .

EXPOSE 8000

USER app

CMD ["npm", "start"]