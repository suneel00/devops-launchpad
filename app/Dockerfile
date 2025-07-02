# Use a lightweight Python image
FROM python:3.9-slim

# Set working directory
WORKDIR /app

# Copy requirements and app source
COPY requirements.txt .
COPY main.py .

# Install dependencies (no cache to keep image small)
RUN pip install --no-cache-dir -r requirements.txt

# Expose Flask port
EXPOSE 5000

# Run the app
CMD ["python3", "main.py"]
