FROM node:20.12.2

WORKDIR /app

COPY ./package.json package.json
COPY ./package-lock.json package-lock.json

RUN npm ci

COPY . .

EXPOSE 8080

CMD ["npm", "run", "build"]