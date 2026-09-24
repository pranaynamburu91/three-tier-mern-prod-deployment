FROM node:alpine

WORKDIR /app

COPY package.json ./

COPY package-lock.json ./

RUN npm ci && npm cache clean --force

COPY . .

CMD ["npm", "start", "--", "--host", "0.0.0.0"]

