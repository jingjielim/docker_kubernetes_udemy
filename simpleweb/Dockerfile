#Specify a base image
FROM node:alpine

# Add all files in our directory into the docker container
WORKDIR /usr/app
COPY ./ ./
# install some dependencies
RUN npm install

# Default command
CMD ["npm", "start"]
