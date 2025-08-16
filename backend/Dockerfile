FROM python:3.11-slim

# Set the working directory
WORKDIR /app

# Install system dependencies if needed (uncomment if you use psycopg2-binary, etc.)
# RUN apt-get update && apt-get install -y build-essential libpq-dev

# Copy the requirements file
COPY requirements.txt ./

# Install the dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy the application files
COPY . .

# Expose Flask port
EXPOSE 5000

# Set environment variables (can be overridden by --env-file)
ENV FLASK_APP=app
ENV FLASK_ENV=development

# Set the command to run the application
CMD ["flask", "run", "--host=0.0.0.0", "--port=5000"]