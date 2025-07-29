# Use official Node.js LTS image
FROM node

# Set working directory inside container
WORKDIR /app

# Copy package.json and package-lock.json (if exists)
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy rest of the source code
COPY . .

# Expose port (5173 is default for Vite)
EXPOSE 5173

# Run the dev server
CMD ["npm", "run", "dev"]
