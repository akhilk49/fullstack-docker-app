# Use Node.js 14 Alpine as base image
FROM node:14-alpine

# Set working directory inside container
WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy all frontend source code
COPY . .

# Expose frontend port
EXPOSE 3000

# Start the frontend server
CMD ["npm", "start"]
