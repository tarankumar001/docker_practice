# Use a lightweight Node.js base image
FROM node:20-alpine

# Create app group and user (non-root)
RUN addgroup app && adduser -S -G app app

# Set working directory
WORKDIR /app

# Copy only package.json files first to leverage Docker layer cache
COPY package*.json ./

# Install dependencies as root
RUN npm install

# Copy the rest of the project files
COPY . .

# Fix permissions for node_modules (Vite writes cache here)
RUN chown -R app:app /app

# Switch to non-root user
USER app

# Expose Vite dev server port
EXPOSE 5173

# Run the dev script
CMD ["npm", "run", "dev"]
