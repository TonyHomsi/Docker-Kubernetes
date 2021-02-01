FROM node

WORKDIR /app
## It is better to use COPY package.json /app in the begining and then RUN npm install
COPY package.json /app

RUN npm install

COPY . /app

EXPOSE 80
##CMD will NOT excute it when the image is created but when the container is started based on the image
CMD ["node", "server.js"]

##To Excute Dockerfile:
# docker build .
# docker run -p 3000:80 <image>
# docker ps // To see the running image
# docker stop <name of the imgae>


