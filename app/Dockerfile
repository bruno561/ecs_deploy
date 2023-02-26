# Use a Node.js base image
FROM node:14

# Create a new directory for the app
WORKDIR /app

# Copy the package.json and package-lock.json files
COPY package*.json ./

# Install app dependencies
RUN npm install

# Copy the rest of the app files
COPY . .

# Expose the port your app listens on (if applicable)
EXPOSE 3000

# Start the app
CMD [ "node", "app.js" ]
