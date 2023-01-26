# kiriDevs/codespaces: TeX

## Key Facts

- **OS:** Alpine Linux
- **Base Image:** Microsoft: VSCode Devontainers `base:alpine`
(`mcr.microsoft.com/devcontainers/base:alpine`)

This devcontainer contains a `texlive` installation and is ready for compiling LaTeX documents out of the box.
It is built on [Alpine Linux](https://alpinelinux.org) to minimize required system storage and computing resource usage

This image does **not** contain any specialised tools (e.g. package managers, build tools) for specific languages on top of the ones already provided in the base image.

## Feature list

- GitHub CLI (pkg: `github-cli`)
- SSH Server (pkg: `openssh`)
- Terminal Editor: NeoVim (`nvim` pkg: `neovim`)
- TeX-Live: Base installation (pkg: `texlive`)
  - Dependencies for `latexindent` that are missing by default

### VSCode Extensions

- Automatically installed: LaTeX Workshop (`James-Yu.latex-workshop`)
