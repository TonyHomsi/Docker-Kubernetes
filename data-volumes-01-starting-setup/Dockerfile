FROM node:14

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

EXPOSE 80

# here is where our data stored and survived
# VOLUME [ "/app/feedback" ] remove it and build it in the terminal! Check the instruction

CMD ["node", "server.js"]