FROM --platform=linux/amd64 ubuntu:24.04
RUN apt update
RUN DEBIAN_FRONTEND=noninteractive apt install -y build-essential binutils gdb sudo
RUN adduser --disabled-password --gecos '' user
RUN echo 'user ALL=(root) NOPASSWD:ALL' > /etc/sudoers.d/user
USER user
WORKDIR /home/user