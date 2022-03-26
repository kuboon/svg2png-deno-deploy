# https://hub.docker.com/_/microsoft-vscode-devcontainers
FROM mcr.microsoft.com/vscode/devcontainers/base:0-ubuntu-21.04

RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
 && apt-get -y install --no-install-recommends fish
RUN chsh -s /usr/bin/fish vscode
USER vscode
SHELL ["/usr/bin/fish", "-l", "-c"]

# http://asdf-vm.com/guide/getting-started.html#_3-install-asdf
RUN git clone https://github.com/asdf-vm/asdf.git ~/.asdf --branch v0.9.0 \
 && mkdir -p ~/.config/fish/completions; and ln -s ~/.asdf/completions/asdf.fish ~/.config/fish/completions \
 && echo "source ~/.asdf/asdf.fish" >> $HOME/.config/fish/config.fish
 
RUN asdf plugin add deno && asdf install deno latest && asdf global deno latest
# RUN deno install -A -f -n land https://deno.land/x/land@v0.7.0/cli.ts

RUN asdf plugin add golang && asdf install golang latest && asdf global golang latest
RUN asdf plugin add rust && asdf install rust latest && asdf global rust latest

RUN asdf reshim
