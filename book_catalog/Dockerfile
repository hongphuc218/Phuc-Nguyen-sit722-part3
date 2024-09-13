# Use an official Python image
FROM python:3.11-slim
# Set the working directory to /app/
WORKDIR /app/

COPY requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

COPY . .
# Run commands when container launch. Set the host IP to 0.0.0.0 and port to 8000
CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "8000"]

