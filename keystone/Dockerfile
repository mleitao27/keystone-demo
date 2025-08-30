# Use official Node.js image
FROM node:20

# Create app directory
WORKDIR /app

# Copy package files
COPY package.json package-lock.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application
COPY . .

# Expose port
EXPOSE 3000

# Start the Keystone app
CMD ["npm", "run", "dev"]
