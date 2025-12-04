FROM python:3.14.1-slim

WORKDIR /tmp

COPY requirements.txt .

RUN apt update && \
    apt -y install \
    gcc \
    build-essential \
    python-dev && \
    python -m pip install --upgrade pip && \
    pip install -r requirements.txt