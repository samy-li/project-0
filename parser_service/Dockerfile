FROM python:3.11
WORKDIR /app

COPY requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

# Create storage directory for file uploads
RUN mkdir -p /app/storage

# Expose the default FastAPI port
EXPOSE 8000


CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "8000"]