# dotfiles

It's a collection of files and directories that I use to setup my development environment.

## Setups

### Shell
Install zsh
```sh
sudo apt install zsh
```

Setup zsh as the default shell
```sh
sudo chsh -s $(which zsh)
```

Install oh-my-zsh
```sh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

Clone spaceship theme
```sh
git clone https://github.com/spaceship-prompt/spaceship-prompt.git "$ZSH_CUSTOM/themes/spaceship-prompt" --depth=1
```

Link spaceship theme
```sh
ln -s "$ZSH_CUSTOM/themes/spaceship-prompt/spaceship.zsh-theme" "$ZSH_CUSTOM/themes/spaceship.zsh-theme"
```

### Node

Install nvm
```sh
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
```

Install latest stable version of node
```sh
nvm install --lts
```

Install yarn
```sh
npm install -g yarn
```

### Git

Add a custom PPA GIT Core
```sh
sudo add-apt-repository ppa:git-core/ppa -y
```

Update apt cache
```sh
sudo apt update
```

Upgrade apt packages
```sh
sudo apt upgrade
```

### Symlinks
Link git config
```sh
ls -s ~/dotfiles/.gitconfig ~/.gitconfig
```

Link zsh config
```sh
ls -s ~/dotfiles/.zshrc ~/.zshrc
```
