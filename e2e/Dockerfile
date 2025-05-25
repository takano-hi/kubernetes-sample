FROM node:24.0.2-bookworm

WORKDIR /app

RUN npx playwright install --with-deps

COPY package.json package-lock.json ./

RUN npm install

COPY . .

CMD ["npm", "run", "test"]
