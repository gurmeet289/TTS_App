# Use an official Python runtime as a parent image
FROM python:3.8-slim

# Set the working directory to /mycode
WORKDIR /mycode

# Copy the current directory contents into the container at /mycode
COPY . /mycode

# Install any needed packages specified in requirements.txt
RUN pip install --trusted-host pypi.python.org -r /mycode/requirements.txt

# Make port 80 available to the world outside this container
EXPOSE 5000

# Define environment variable
ENV NAME World

# Run app.py when the container launches
CMD ["python", "/mycode/main.py"]
