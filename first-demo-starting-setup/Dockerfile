# node 14 as base image
FROM node:14

# certain directory in the container
WORKDIR /app

# copy the package.json into container
COPY package.json .

# install all the dependecies
RUN npm install

# copy the rest of the code into the container
COPY . .

# open 3000 port to the outside world
EXPOSE 3000

# these are node command
CMD [ "node", "app.mjs" ]

# docker 
#9991ee1fb0072b6906474a8bd5a271075c5ced1ab57ba

