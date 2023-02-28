# Use the latest LTS (long-term support) version of Node.js as the base image
FROM docker.io/node:lts

# Set the working directory to the project root
WORKDIR /app

# Copy the package.json and package-lock.json files to the working directory
COPY package*.json ./

# Install the dependencies
RUN npm install

# Copy the rest of the project files to the working directory
COPY . .

# Expose the app's port
EXPOSE 3000

# Run the app when the container is started
CMD [ "npm", "start" ]
