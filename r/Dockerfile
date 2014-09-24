#
# R Dockerfile
#
# https://github.com/mixxen/dockerfile
#

# Pull base image.
FROM ubuntu:14.04

RUN \ 
  apt-get update && \
  apt-get install -y r-base && \
  apt-get install -y r-base-dev && \
  rm -rf /var/lib/apt/lists/*

# Define working directory.
WORKDIR /workspace

CMD ["R"]

