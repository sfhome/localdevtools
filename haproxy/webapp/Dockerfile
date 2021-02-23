FROM python:3.8.8-slim-buster

WORKDIR /app
COPY requirements.txt .
RUN pip install -r requirements.txt
COPY main.py .

ENTRYPOINT [ "uvicorn", "main:app", "--host", "0.0.0.0" ]
