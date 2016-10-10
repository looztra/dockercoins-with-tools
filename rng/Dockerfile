FROM python:alpine
RUN apk add --update --no-cache \
    wget \
    curl \
    netcat-openbsd \
    net-tools
RUN pip install Flask
COPY rng.py /
CMD ["python", "rng.py"]
EXPOSE 80
