# Use a Node.js LTS version as the base image
FROM node:lts

# Set the working directory to /app
WORKDIR /app

# Copy the package.json and package-lock.json files to the container
COPY package*.json ./

# Install the dependencies from package.json
RUN npm install

# Copy the rest of the application files to the container
COPY . .

# Expose port 3000 for the server
EXPOSE 3000

# Start the server using Node.js
CMD [ "node", "app.js" ]
