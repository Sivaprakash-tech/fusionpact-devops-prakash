# backend/Dockerfile
FROM python:3.11-slim

ENV PYTHONDONTWRITEBYTECODE=1
ENV PYTHONUNBUFFERED=1

WORKDIR /app

# copy requirements and install
COPY requirements.txt /app/requirements.txt
RUN pip install --no-cache-dir -r /app/requirements.txt

# copy the application code
COPY . /app

# create data folder with correct permissions
RUN mkdir -p /app/app/data && chmod -R 777 /app/app/data

EXPOSE 8000

# Run uvicorn (app entrypoint is app.main:app per your provided file)
CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "8000", "--workers", "1"]
