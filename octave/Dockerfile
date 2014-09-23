#
# Octave Dockerfile
#
# https://github.com/mixxen/dockerfile
#

# Pull base image.
FROM ubuntu:14.04

RUN \ 
  apt-get update && \
  apt-get install -y octave && \
  rm -rf /var/lib/apt/lists/*

# Define working directory.
WORKDIR /workspace

CMD ["octave"]

