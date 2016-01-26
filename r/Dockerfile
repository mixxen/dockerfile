#
# R Dockerfile
#
# https://github.com/mixxen/dockerfile
#

# Pull base image.
FROM ubuntu:14.04

RUN sh -c 'echo "deb http://cran.rstudio.com/bin/linux/ubuntu trusty/" >> /etc/apt/sources.list'
RUN gpg --keyserver keyserver.ubuntu.com --recv-key E084DAB9
RUN gpg -a --export E084DAB9 | sudo apt-key add -

RUN \ 
  apt-get update && \
  apt-get install -y r-base && \
  apt-get install -y r-base-dev && \
  apt-get install -y libcurl4-openssl-dev && \
  rm -rf /var/lib/apt/lists/*

RUN R -e "install.packages('devtools', repos = 'http://cran.rstudio.com/')"

# Define working directory.
WORKDIR /workspace

CMD ["R"]

