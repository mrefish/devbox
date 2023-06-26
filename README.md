# devbox

# Installation
```shell
# Install Nix
curl --proto '=https' --tlsv1.2 -sSf -L https://install.determinate.systems/nix | sh -s -- install

# Enable Nix Flakes
mkdir -p ~/.config/nix
echo "experimental-features = nix-command flakes" >> ~/.config/nix/nix.conf

# Install Devbox
curl -fsSL https://get.jetpack.io/devbox | bash

# Install Fleek
curl -fsSL https://getfleek.dev/installer | bash
```


# Setup
```shell
# Pull the Fleek profile
devbox global pull https://devbox.getfleek.dev/high

# Pull this repo's config
devbox global pull https://raw.githubusercontent.com/mrefish/devbox/main/devbox.json

# Add Devbox to .rc file
devbox global run install-hook-bash
```
