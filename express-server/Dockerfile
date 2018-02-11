FROM node:8.9-alpine
# Create a directory where our app will be placed
RUN mkdir -p /usr/src/app

WORKDIR /usr/src/app
# Copy dependency definitions
COPY package.json /usr/src/app

RUN npm install
# Get all the code needed to run the app
COPY . /usr/src/app

EXPOSE 3000

# Serve the app
CMD ["npm", "start"]