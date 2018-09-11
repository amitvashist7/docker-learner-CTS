# Base Image to build the Container Image.
FROM ubuntu:latest

# Who is maintaing this image.
MAINTAINER Amit Vashist <amitvashist7@gmail.com>

# Build the basic Apache Server on Ubuntu
RUN apt-get update

# Install Apache Package with Apt-Get
RUN apt-get install apache2 -y

# Copy the Custom Index Page
COPY index.html /var/www/html/

# Expose the Service
EXPOSE 80 

# Bring the Apache Service
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND" ]
