# Use an official Node.js image as the base
FROM node:16-alpine

# Set the working directory
WORKDIR /app

# Copy package.json and package-lock.json
COPY backend/package*.json ./

# Install dependencies
RUN npm install

# Copy the back-end code
COPY backend/ .

# Expose the server port
EXPOSE 5000

# Set the default command to start the server
CMD ["node", "server.js"]
