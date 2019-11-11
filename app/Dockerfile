FROM node:8

ENV HTTP_PROXY "http://194.145.60.1:9400"
ENV HTTPS_PROXY "http://194.145.60.1:9400"

WORKDIR /usr/src/app
RUN pwd
COPY app/* ./
RUN ls -l
RUN npm ci --only=production

EXPOSE 8080
CMD [ "npm", "start" ]
