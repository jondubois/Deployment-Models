# 1. Pulling the docker images we need
FROM python:2.7.11
MAINTAINER Stephen Rodriguez <@stephnr>

# 2. Labelling the docker image version/details
LABEL version="1.0"
LABEL description="Simple Static Website Dockerfile using Python. Runs local web server from project root"

###################################
######      SETUP STACK      ######
###################################

# 3. Setup the application folder
RUN mkdir -p /usr/src/app

# 4. Change our working directory
WORKDIR /usr/src/app

# 6. Provide Environment Properties
# ENV ...

# 7. Copy project files into the application folder
COPY . /usr/src/app

# Step 8 ignored since static app

# 9. Your Custom Build Steps
# {{ CUSTOM BUILD STEPS GO HERE }}

###################################
######      EXPOSE PORT      ######
###################################

# 10. Expose the app on port 80
EXPOSE 80

###############################
######      RUN APP      ######
###############################

# 11. Run the application specific build/run commands
CMD [ "python", "-m", "SimpleHTTPServer", "80" ]
