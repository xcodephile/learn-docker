# Specify a base image
FROM node:alpine

WORKDIR /usr/app

# Install some depenendencies
COPY ./package.json ./
RUN npm install

# Place this line after npm install to minimizing cache busting
COPY ./ ./

# Default command
CMD ["npm", "start"]