# Specify base image
FROM node:14-alpine

WORKDIR /usr/app

##  Install dependencies

# Segment of packages
COPY ./package.json ./
RUN npm install

# Remainder of files that not interfere with my run npm
# This is an action to minimize cache busting

COPY ./ ./

# Default Command

CMD ["npm", "start"]