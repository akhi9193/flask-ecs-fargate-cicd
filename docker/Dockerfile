# Use the official Python image from the Docker Hub
FROM python:3.9-slim

# Set the working directory inside the container
WORKDIR /app

# Copy the requirements file into the container
COPY app/requirements.txt .

# Install the dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy the Flask app code into the container
COPY app/ /app/

# Expose port 5000 for the Flask app
EXPOSE 5000

# Define the command to run the Flask app
CMD ["python", "app.py"]
