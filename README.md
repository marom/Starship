# Starship
customizable prompt for any shell!

Prerequisites
A Nerd Font (opens new window)installed and enabled in your terminal 


Step 1. Install Starship

LINUX
Install the latest version for your system:
curl -sS https://starship.rs/install.sh | sh


WINDOWS
Install Starship using any of the following package managers:

Repository	Instructions
crates.io	cargo install starship --locked
Chocolatey	choco install starship
conda-forge	conda install -c conda-forge starship
Scoop		scoop install starship

Step 2. Setup your shell to use Starship

Bash
Add the following to the end of ~/.bashrc:
eval "$(starship init bash)"

Cmd
You need to use Clink (opens new window)(v1.2.30+) with Cmd. Create a file at this path %LocalAppData%\clink\starship.lua with the following contents:

load(io.popen('starship init cmd'):read("*a"))()

Zsh
Add the following to the end of ~/.zshrc:

eval "$(starship init zsh)"

Restart your terminal and it's DONE!!

