# Use Node.js base image
FROM node:14-alpine

# Set working directory
WORKDIR /usr/src/app

# Copy package.json first
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy rest of the app
COPY . .

# Expose frontend port
EXPOSE 3000

# Start the React dev server
CMD ["npm", "start"]
