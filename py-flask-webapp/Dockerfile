# Use an official Python runtime as base image
FROM python:3.11-slim

# Set the working directory
WORKDIR /app

# Copy the current directory contents into the container
COPY . .

RUN python -m pip install --upgrade pip

# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Expose the port Flask will run on
EXPOSE 5000

# Run the Flask app
CMD ["python", "app.py"]

