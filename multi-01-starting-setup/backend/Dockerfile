FROM node

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

EXPOSE 80

ENV MONGODB_USERNAME=Tony
ENV MONGODB_PASSWORD=secure

CMD ["npm", "start"]