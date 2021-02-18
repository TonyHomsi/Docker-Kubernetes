FROM node:14


WORKDIR /app

COPY package.json .

RUN npm install

# We could remove COPY . . if we are using the bind mount
COPY . .

ARG DEFAULT_PORT=80

ENV PORT $DEFAULT_PORT

EXPOSE $PORT

# here is where our data stored and survived
# VOLUME [ "/app/feedback" ] remove it and build it in the terminal! Check the instruction

# You can add [" /app/node_modules"]
CMD ["npm", "start"]