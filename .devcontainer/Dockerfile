FROM mcr.microsoft.com/devcontainers/base:ubuntu-24.04
RUN apt-get update && \
    apt-get install -y  \
    libreadline-dev zlib1g-dev libxml2-dev libxslt-dev \ 
    libssl-dev libxml2-utils libc-dev libipc-run-perl \ 
    python3 python3-poetry \
    build-essential xsltproc flex bison ccache meson gdb vim
RUN useradd -ms /bin/bash pg-dev && \
    echo pg-dev ALL=\(root\) NOPASSWD:ALL > /etc/sudoers.d/pg-dev && \
    chmod 0440 /etc/sudoers.d
USER pg-dev