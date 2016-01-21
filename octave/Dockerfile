#
# Octave Dockerfile
#
# https://github.com/mixxen/dockerfile
#

# Pull base image.
FROM ubuntu:14.04

RUN \ 
  apt-get update && \
  apt-get install -y software-properties-common && \
  apt-get install -y build-essential && \
  apt-add-repository ppa:octave/stable && \
  apt-get update && \
  apt-get install -y octave && \
  apt-get install -y epstool && \
  apt-get install -y transfig && \
  apt-get install -y liboctave-dev && \
  rm -rf /var/lib/apt/lists/*

# Define working directory.
WORKDIR /workspace

CMD ["octave"]
