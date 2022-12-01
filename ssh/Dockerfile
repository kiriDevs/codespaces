FROM mcr.microsoft.com/vscode/devcontainers/base:buster

ARG nvimTag=stable

RUN apt update && apt install -y \
    ninja-build gettext libtool libtool-bin autoconf \
    automake cmake g++ pkg-config unzip curl doxygen
RUN cd /tmp/ \
    && git clone https://github.com/neovim/neovim \
    && git -C ./neovim/ checkout $nvimTag
RUN cd /tmp/neovim/ \
    && make CMAKE_BUILD_TYPE=Release \
    && make install