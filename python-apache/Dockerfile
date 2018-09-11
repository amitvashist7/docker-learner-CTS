# Base Image to build the Container Image.
FROM python:2.7-slim

# Who is maintaing this image.
MAINTAINER Amit Vashist <amitvashist7@gmail.com>

# Set the Working Dir. 
WORKDIR /app

# Copy the Current Dir Content inside the Container
ADD . /app

# Install any needed packages
RUN pip install --trusted-host pypi.python.org -r req.txt

# Expose the Service
EXPOSE 80 

# ENV Vairiable
ENV NAME World


# Bring the Apache Service
CMD ["python", "app.py" ]
