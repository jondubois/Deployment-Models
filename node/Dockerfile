###################################
######      SETUP STACK      ######
###################################
FROM node:5.11.0

# Create the app directory
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

# Install npm dependencies
COPY package.json /usr/src/app

# Changes your node execution environment
ENV NODE_ENV=development
RUN npm install --production

# Bundle app source
COPY . /usr/src/app

###################################
######      EXPOSE PORT      ######
###################################

# Open the http port
EXPOSE 8080

###############################
######      RUN APP      ######
###############################

# Start the app
CMD [ "npm", "start" ]
