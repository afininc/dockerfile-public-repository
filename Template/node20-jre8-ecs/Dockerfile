FROM public.ecr.aws/afininc/node20-jre8-alpine-base:latest
WORKDIR /usr/src/app
ARG ENV

ENV TZ=Asia/Seoul

COPY . .
RUN yarn set version berry

RUN yarn cache clean
RUN yarn install

RUN echo $ENV
RUN if [ "$ENV" = "prod" ]; then yarn build:prod; fi
RUN if [ "$ENV" = "dev" ]; then yarn build:dev; fi
RUN if [ "$ENV" = "local"]; then yarn build:local; fi

EXPOSE 80
CMD [ "yarn", "start" ]
