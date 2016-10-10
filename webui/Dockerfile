FROM node:4-slim
RUN apt-get update \
    && apt-get install -y \
       wget \
       curl \
       netcat \
       dnsutils 
RUN npm install express
RUN npm install redis
COPY files/ /files/
COPY webui.js /
CMD ["node", "webui.js"]
EXPOSE 80
