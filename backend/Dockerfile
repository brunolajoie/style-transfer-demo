# backend/Dockerfile

FROM python:3.10.1-slim

WORKDIR /app

RUN apt-get update

# 'ffmpeg', 'libsm6', and 'libxext6' are required for OpenCV.
RUN apt-get install \
    'ffmpeg'\
    'libsm6'\
    'libxext6'  -y

COPY requirements.txt .
RUN pip install -r requirements.txt

COPY . .

EXPOSE 8080

CMD ["python", "main.py"]
