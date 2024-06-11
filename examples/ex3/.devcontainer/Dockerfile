ARG TAG="4.4.0"

FROM  rocker/r-base:$TAG

RUN apt-get update && apt-get install -y --no-install-recommends vim

RUN mkdir settings

COPY install_packages.R /settings

RUN Rscript 'settings/install_packages.R'