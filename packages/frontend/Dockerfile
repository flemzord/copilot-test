FROM node:14-alpine

WORKDIR /app

COPY . /app/
RUN yarn install --silent

RUN yarn build

EXPOSE 3000

ENV NUXT_HOST=0.0.0.0
ENV NUXT_PORT=3000

# start the app
CMD [ "yarn", "start" ]
