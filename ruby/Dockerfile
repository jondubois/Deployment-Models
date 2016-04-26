# 1. Pulling the docker images we need
FROM ruby:2.1
MAINTAINER Stephen Rodriguez <@stephnr>

# 2. Labelling the docker image version/details
LABEL version="1.0"
LABEL description="Simple Python 2.x Dockerfile. Executes `fab start` to run your app"

###################################
######      SETUP STACK      ######
###################################

# Step 3-8 are done earlier in the `ruby:2.1` image

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
CMD [ "rake" ]
