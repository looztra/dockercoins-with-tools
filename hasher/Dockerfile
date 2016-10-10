FROM ruby:alpine
RUN apk add --update --no-cache \
    build-base \
    wget \
    curl \
    netcat-openbsd \
    net-tools
RUN gem install sinatra
RUN gem install thin
ADD hasher.rb /
CMD ["ruby", "hasher.rb"]
EXPOSE 80
