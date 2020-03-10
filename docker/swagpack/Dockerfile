FROM node:12.13.1

WORKDIR /app

RUN yarn init -y
RUN yarn global add swagpack

CMD [ "swagpack", "build", "./src/index.yml", "-o", "/app/spec.yml", "-w", "./src" ]
