# Use Python 3.12 as the base image
FROM python:3.12

# Set the working directory
WORKDIR /data

# Install system dependencies
RUN apt-get update && apt-get install -y python3-pip

# Install setuptools explicitly (fixes the distutils issue)
RUN pip install --no-cache-dir setuptools

# Install Django
RUN pip install --no-cache-dir django==3.2

# Copy project files into the container
COPY . .

# Expose port 8000
EXPOSE 8000

# Start the Django server
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
