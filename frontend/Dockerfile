FROM node:16
WORKDIR /app
COPY package.json .
RUN npm install
COPY . .
ENV NODE_APP_BACKEND_URL https://backend.karunaduflavors.com
RUN npm run build

CMD ["npx", "serve", "-s", "build", "-l", "3000"]
