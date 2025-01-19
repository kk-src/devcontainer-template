FROM mcr.microsoft.com/devcontainers/base:ubuntu-24.04
RUN apt-get update && apt-get install -y build-essential libreadline-dev zlib1g-dev flex bison libxml2-dev libxslt-dev libssl-dev libxml2-utils xsltproc ccache meson libipc-run-perl gdb libc-dev vim
RUN useradd -ms /bin/bash pg-dev && usermod -aG sudo pg-dev
USER pg-dev
