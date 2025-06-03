FROM node:18.9.1


WORKDIR /app

# Copy the file from your host to your current location
COPY package.json .

# Run the command inside your image filesystem
RUN npm install

# Inform Docker that the container is listening on the specified port at runtime
EXPOSE 5173

# Copy the rest of your app's source code from your host to your image filesystem
COPY . .

# Run the specified command within the container
CMD ["npm", "run", "dev"]
