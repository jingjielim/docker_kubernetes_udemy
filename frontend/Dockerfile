FROM node:alpine as builder

WORKDIR '/app' 

COPY package.json .
RUN npm install

COPY . . 

RUN npm run build

# adding a new FROM command signals a new stage 
FROM nginx
COPY --from=builder /app/build  /usr/share/nginx/html
# Default command in nginx will start up nginx for us