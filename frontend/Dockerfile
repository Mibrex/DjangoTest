# Base image
FROM node:18-alpine

# Set the working directory
WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

# Set environment variables
ENV PORT=3000
ENV HOST=0.0.0.0

# Expose the port on which the React app will run
EXPOSE $PORT

# Start the development server
CMD ["npm", "start"]
