# Use the official Node.js image as base
FROM node:alpine

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json (assuming they are directly in the ./api directory)
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application (assuming the rest of your source code is directly in the ./api directory)
COPY . .

# Expose port 3000 to the outside world
EXPOSE 3000

# Command to run the application
CMD ["node", "server.js"]
