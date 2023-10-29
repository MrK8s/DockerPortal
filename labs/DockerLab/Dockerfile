# Use the official Python image as a base image
FROM python:3.9-slim

# Set the working directory inside the container
WORKDIR /app

# Copy requirements.txt and install Python dependencies
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy the Flask application to the container
COPY app.py .

# Expose port 5000 for the application
EXPOSE 5000

# Command to run the application
CMD ["python", "app.py"]
