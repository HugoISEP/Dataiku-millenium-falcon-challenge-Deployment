FROM node:16-alpine
WORKDIR /app
COPY build ./build
RUN yarn global add serve
EXPOSE 3000
CMD [ "serve", "-s", " build" ]
