#Specify a base image
FROM node:alpine

# Add all files in our directory into the docker container
WORKDIR /usr/app
COPY ./package.json ./
# install some dependencies
RUN npm install 
COPY ./ ./

# Default command
CMD ["npm", "start"]
