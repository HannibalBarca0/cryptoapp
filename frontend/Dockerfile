# Use the official Node.js image as the base image
FROM node:20

# Set working directory
WORKDIR /usr/src/app

# Copy frontend package files and install dependencies (if using npm)
COPY package*.json ./
RUN npm install

# Copy the frontend source code
COPY . .

# Build the static assets (adjust if your project uses a different build command)
RUN npm run build

# Expose port (adjust according to your project configuration, e.g., if using serve in production)
EXPOSE 3000

# Start the application (adjust command for production server)
CMD ["npm", "run", "start"]