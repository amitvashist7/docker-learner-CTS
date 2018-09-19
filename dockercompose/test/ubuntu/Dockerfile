# Base Image 
FROM ubuntu:latest

# Who is managing this images/ file
MAINTAINER Amit Vashist <amitvashist7@gmail.com>

# Update the Apt-Get Repo
RUN apt-get update

# Install the Apache Packages
RUN apt-get install apache2 -y 

# Volumes 
VOLUME [ "/var/www/html" ]

# Working Dir
WORKDIR /var/www/html

# Setup a Test Web Page
COPY abc.html /var/www/html/abc.html

# Expose the Apache Web
EXPOSE 80

# Bring the Apache Up inside the container
CMD [ "/usr/sbin/apache2ctl", "-D", "FOREGROUND" ]
