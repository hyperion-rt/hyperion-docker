# The aim of this docker image is to set up an environment in which we can run
# the Hyperion bit-level tests, to make sure that changes are not due to any
# changes in environment but only changes in the code itself. This image uses
# HDF5 1.10.x

FROM ubuntu:18.04
MAINTAINER Thomas P. Robitaille <thomas.robitaille@gmail.com>

# We set up all the Fortran dependencies using apt-get rather than use e.g.
# conda, to have as standard an environment as possible. We leave the installation
# of the Python dependencies to CircleCI
RUN apt-get update
RUN apt-get install -y libmpich-dev \
                       libhdf5-serial-dev \
                       python3-dev \
                       python3-setuptools \
                       python3-pip \
                       git \
                       make

RUN mkdir -p /root/.config/matplotlib
RUN echo "backend: Agg" > /root/.config/matplotlib/matplotlibrc
