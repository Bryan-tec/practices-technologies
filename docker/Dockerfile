FROM ubuntu:latest

RUN apt-get update && apt-get install -y \
    python3 \
    python3-pip \
    apt-get install -y nodejs \
    npm \
    && rm -rf /var/lib/apt/lists/*

WORKDIR /app

COPY practices-technologies/docker/requirements.txt .

RUN pip3 install --no-cache-dir -r requirements.txt
CMD ["python3", "app.py"]

EXPOSE 8080
