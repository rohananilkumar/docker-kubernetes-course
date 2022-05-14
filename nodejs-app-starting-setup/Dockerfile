# --- All of these are run at the time of building of the image

FROM node
#from node image (can either exist locally or on the docker hub)

WORKDIR /app
#tells docker to execute all the commands from the /app directory

COPY package.json /app

RUN npm install
#asks docker to run npm install on the /app directory

COPY . /app
#this specifies that all the project files should be copied onto the /app directory of the docker container


# --- All of these are run at the time of starting of a container

EXPOSE 80
#this exposes port 80 on the docker container to the host machine

CMD ["node", "server.js"]
#runs the ,server js file