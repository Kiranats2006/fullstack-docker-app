# Use Node.js base image
FROM node:14-alpine

# Set working directory
WORKDIR /usr/src/app

# Copy package.json first (better for caching)
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the app
COPY . .

# Expose backend port
EXPOSE 5000

# Start the app
CMD ["npm", "start"]
