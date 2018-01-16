# Set the base image
FROM ubuntu

# Dockerfile author / maintainer 
MAINTAINER Name yajananrao@gmail.com

# To fix error
RUN apt-get update && apt-get install -y --no-install-recommends apt-utils

# Update application repository list and install the java
RUN apt-get update && apt-get install -y default-jre && apt-get -y install openjdk-8-jdk

# Installing python
RUN apt-get -y install python2.7 && apt-get -y install python-pip

# Updating pip
RUN pip install --upgrade pip

# Installing taurus
RUN pip install bzt

#Installing chrome-stable
RUN apt-get -y install wget
RUN wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
RUN dpkg -i google-chrome-stable_current_amd64.deb; apt-get -fy install
