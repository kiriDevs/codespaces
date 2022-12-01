# kiriDevs/codespaces: SSH

## Key Facts

- **OS:** Debian 10 ("Buster")
- **Base Image:**  Microsoft: VSCode Devontainers `base:buster`
(`mcr.microsoft.com/vscode/devcontainers/base:buster`)

This Devcontainer image is intended to quickly provide a development experience for the command line, without a graphical editor.
Next to an SSH sever to allow for connecting from the terminal, it contains general CLIs and a terminal-based text editor.

This image does **not** contain any specialised tools (e.g. package managers, build tools) for specific languages on top of the ones already provided in the base image.

## Feature list

- GitHub CLI
- SSH Server (`sshd`)
- Terminal Editor: [NeoVim (`nvim`)](https://github.com/neovim/neovim) - built form source at build time

## Docker build arguments

Argument | Default | Description
--- | --- | ---
`nvimTag` | `stable` | The `git` tag of the desired `neovim` version (see list at https://github.com/neovim/neovim)
