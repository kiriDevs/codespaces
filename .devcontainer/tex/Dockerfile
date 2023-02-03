FROM alpine:3.17

# Install miscellaneous packages
RUN apk add --no-cache github-cli openssh neovim

# Dependencies for latexindent
RUN apk add --no-cache perl-yaml-tiny make \
    && perl -MCPAN -e 'install "File:HomeDir"'

# Install texlive itself
RUN apk add --no-cache texlive