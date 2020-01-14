FROM ruby:2.6.0

WORKDIR /usr/src/
COPY . .


RUN apt-get update -qq \
  && apt-get install libxml2-dev \
  libxslt-dev \
  sqlite3 \
  -yy nodejs \
  && rm -rf /var/cache/apk/*
RUN gem install bundler:1.17.2
RUN bundle config build.nokogiri --use-system-libraries
RUN bundle install
RUN rails db:migrate

ENTRYPOINT rails s 
