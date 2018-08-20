FROM python:2.7-slim

# Set working dir to app
WORKDIR /app

# Copy the current dir contents to the container at /app
ADD . /app

# Install any needed packages specified in requirements.txt
RUN pip install --trusted-host pypi.python.org -r requirements.txt

#Make port 80 available to the world outside this container
EXPOSE 80

# define environment variable
ENV NAME world

#Run app.py when the container launches
CMD ["python", "app.py"]
