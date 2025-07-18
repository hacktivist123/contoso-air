FROM node:22-alpine

ENV PORT=3000


WORKDIR /usr/src/app

COPY src/web/package*.json ./

RUN npm ci --omit=dev
COPY src/web .

EXPOSE 3000
CMD ["npm", "start"]
