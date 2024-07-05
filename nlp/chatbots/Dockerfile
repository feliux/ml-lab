FROM python:3.13.0b2-slim

WORKDIR /tmp

COPY requirements.txt .

RUN apt update && \
    apt -y install \
    gcc \
    build-essential \
    python-dev && \
    python -m pip install --upgrade pip && \
    pip install -r requirements.txt