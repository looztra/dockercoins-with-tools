FROM python:alpine
RUN apk add --update --no-cache \
    wget \
    curl \
    netcat-openbsd \
    net-tools
RUN pip install redis
RUN pip install requests
COPY worker.py /
CMD ["python", "worker.py"]
