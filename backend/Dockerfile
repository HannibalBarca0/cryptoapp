# Use the official Node.js image as the base image
FROM node:20

# Set the working directory
WORKDIR /usr/src/app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the backend code
COPY . .

# Expose application port (adjust as needed, e.g., 3000)
EXPOSE 3000

# Start the application (adjust this command based on your start script)
CMD ["npm", "run", "start"]