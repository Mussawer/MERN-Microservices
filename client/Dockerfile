#base image
FROM node:alpine

#setting working directory in container
WORKDIR /app

#copy package.jsonfile to workdir
COPY package.json ./

#run npm install to install all the dependencies
RUN npm install

#copy everything from post directory and paste it to workdir 
COPY ./ ./

#send default run command
CMD [ "npm", "start" ]
