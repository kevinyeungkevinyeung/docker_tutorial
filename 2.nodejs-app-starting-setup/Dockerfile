FROM node

# setting the working directory
WORKDIR /app

# ensure the npm install will come before the source code layer
COPY package.json /app

RUN npm install

# first . means all the files in the same folder as the Dockerfile (all folder and sub folder)
# second ./ means to current directory inside the docker
COPY . /app

# expose a port to outside the container
# for documentation purpose only, is useless
EXPOSE 80

# CMD will not run when image is built, but when the container is start
CMD ["node", "server.js"]