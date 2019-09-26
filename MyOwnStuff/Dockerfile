# Use a Node image. Can easily find other images in the internet.
FROM node:latest

#https://docs.docker.com/engine/reference/builder/#workdir
#WORKDIR essentially initializes sort of a workplace for your Docker container.
#So that whatever actions like COPY happens there.
WORKDIR /app

#https://docs.docker.com/engine/reference/builder/#copy
#Essentially, COPY adds the specified files to Docker container's file system.
COPY . /app

#https://docs.docker.com/engine/reference/builder/#run
#RUN will run the given command WITHIN the Docker container image.
RUN node checkBuild.js

#https://docs.docker.com/engine/reference/builder/#cmd
#Configures the commands when the container is starts to run.
CMD ["node", "sayHello.js"]
