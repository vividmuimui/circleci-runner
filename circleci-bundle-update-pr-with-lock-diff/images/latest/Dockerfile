FROM circleci/ruby:latest
RUN gem update --system && \
    gem update bundler --no-document && \
    gem install circleci-bundle-update-pr lock_diff --no-document
ADD build.sh /usr/local/bin/build
RUN sudo chmod +x /usr/local/bin/build
