FROM ruby:2.1.5

RUN apt-get update && apt-get -y install npm --no-install-recommends

WORKDIR /tmp
COPY Gemfile /tmp
COPY Gemfile.lock /tmp
RUN bundle install
RUN rm /tmp/Gemfile*

