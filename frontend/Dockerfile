FROM node:10

COPY . .

RUN npm install \
    && npm run build

EXPOSE 3000

#or CMD command
ENTRYPOINT npm run start
