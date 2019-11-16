FROM ruby:2.5.0

ADD . /app
WORKDIR /app
RUN bundle install --jobs=8 --without development
CMD ["unicorn", "-c", "./config/unicorn.rb"]
