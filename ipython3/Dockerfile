#
# Python3 Dockerfile
#
# https://github.com/mixxen/dockerfile
#

# Pull base image.
FROM ubuntu:14.04

RUN \
  apt-get update && \
  apt-get install -y python3 && \
  apt-get install -y ipython3 python3-numpy python3-scipy python3-matplotlib ipython3-notebook python3-pandas python3-nose python3-pip && \
  pip3 install sympy && \
  rm -rf /var/lib/apt/lists/* && \
  apt-get autoremove -y

# Define working directory.
WORKDIR /workspace

CMD ["ipython3"]
