#Initializing the containerization process by selecting a base image.
FROM node:20-alpine

#Create and set the working directory
WORKDIR /usr/src/app

#Copy package.json inside the working directory
COPY package*.json ./

#Install the dependencies inside package.json
RUN npm install

#Copy the rest of the app(app.js)
COPY . .

#Expose this microservice at given PORT
EXPOSE 3003

CMD [ "npm" , "start"]