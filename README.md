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
```


# Setup
```shell
# Pull this repo's config
devbox global pull https://raw.githubusercontent.com/mrefish/devbox/main/devbox.json

# Add Devbox to .rc file
echo 'eval "$(devbox global shellenv)"' > ~/.bashrc
```

# Pretty (basic)
```shell
# Get this themey thing
curl https://raw.githubusercontent.com/riobard/bash-powerline/master/bash-powerline.sh > ~/.bash-powerline.sh

# Put it in .rc
echo 'source ~/.bash-powerline.sh` > ~/.bashrc
```
