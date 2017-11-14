# Set up StarCraft II Learning Environment
# docker run -e \
#        DISPLAY=$(ifconfig en0 | grep 'inet ' | cut -d" " -f):0
#        --name xeyes
# Use an official Ubuntu release as a base image
FROM ubuntu:trusty
LABEL maintainer="Elaine Yeung <yeung.egs@gmail.com>"

# Update apt-get and install x11-apps
RUN apt-get update --assume-yes --quiet=2
RUN apt-get install --assume-yes --quiet=2 x11-apps

# Launch xeyes app
CMD xeyes
