# Step 1: Use an official Node.js runtime as a parent image
FROM debian:bullseye-slim

# Step 2: Set the working directory inside the container
WORKDIR /usr/src/app

# Step 3: Copy package.json and package-lock.json for npm install
COPY package*.json ./

# Step 4: Install dependencies
RUN npm install

# Step 5: Copy the rest of the application files
COPY . .

# Step 6: Expose the port your app runs on (default Node.js port is 3000)
EXPOSE 3000

# Step 7: Define the command to run your app
CMD ["node", "app.js"]
