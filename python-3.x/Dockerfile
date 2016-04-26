# 1. Pulling the docker images we need
FROM python:3.5.1
MAINTAINER Stephen Rodriguez <@stephnr>

# 2. Labelling the docker image version/details
LABEL version="1.0"
LABEL description="Simple Python 2.x Dockerfile. Executes `fab start` to run your app"

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

# 8. Install Dependencies (not devDependencies)
RUN pip install --no-cache-dir -r requirements.txt

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
CMD [ "fab", "start" ]
