FROM node:8

WORKDIR /usr/src/app
RUN pwd
COPY app/package*.json ./
RUN ls -l
RUN npm ci --only=production

COPY . .

EXPOSE 8080
CMD [ "npm", "start" ]
