FROM ubuntu:latest

# Update and upgrade APT
RUN apt-get update
RUN apt-get upgrade -y

# Install Python3, pip3, and dependencies
RUN apt-get install -y python3 python3-pip

# Remove externally managed environment warning
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED

# Install Flask and Flask-CORS using pip3
RUN pip3 install flask
RUN pip3 install flask-cors

# Set the working directory
WORKDIR /app

# Copy the Python file into the container
COPY api.py /app

# Run the Flask app
CMD python3 api.py
