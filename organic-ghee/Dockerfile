# Use Node.js LTS
FROM node:18-alpine

# Set working directory
WORKDIR /usr/src/app

# Copy dependency files first
COPY package*.json ./

# Install only production dependencies
RUN npm install

# Copy the rest of the code
COPY . .

# Set environment variables
ENV PORT=3000

# Expose app port
EXPOSE 3000

# Start the app
CMD ["node","app.js"]
