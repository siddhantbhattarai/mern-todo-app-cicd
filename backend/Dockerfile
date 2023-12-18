# Use an official Node runtime as a base image
FROM node:14-alpine

# Set the working directory in the container
WORKDIR /usr/src/app/backend

# Copy package.json and package-lock.json to the container
COPY package*.json ./

# Install backend dependencies
RUN npm install

# Install nodemon globally
RUN npm install -g nodemon

# Copy the rest of the application files to the container
COPY . .

# Expose the port your app will run on
EXPOSE 8000

# Command to run the application using nodemon
CMD ["nodemon", "server.js"]
