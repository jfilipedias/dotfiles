# dotfiles

It's a collection of files and directories that I use to setup my development environment.

## How to use it
Clone this repository:
```sh
git clone git@github.com:jfilipedias/dotfiles.git "$HOME/.dotfiles" --depth=1
```

Run the following command to make the symbolic links:

```sh
ln -s ~/.dotfiles/.gitconfig ~/.gitconfig
ln -s ~/.dotfiles/.zshrc ~/.zshrc
```


## Setups

### Shell
Install zsh on Ubuntu: 
```sh
sudo apt install zsh
sudo chsh -s $(which zsh)
```

Install zsh on Fedora: 
```sh
sudo dnf install zsh
sudo dnf install utils-linux-user
sudo chsh -s $(which zsh)
```

Install oh-my-zsh:
```sh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

Adds the spaceship theme to oh-my-zsh:
```sh
git clone https://github.com/spaceship-prompt/spaceship-prompt.git "$ZSH_CUSTOM/themes/spaceship-prompt" --depth=1

ln -s "$ZSH_CUSTOM/themes/spaceship-prompt/spaceship.zsh-theme" "$ZSH_CUSTOM/themes/spaceship.zsh-theme"
```

Set `ZSH_THEME="spaceship"`  in your `.zshrc`.

### Node

Install nvm:
```sh
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
```

Install latest stable version of node:
```sh
nvm install --lts
```

Install yarn:
```sh
npm install -g yarn
```

### Git

Updates git on Ubuntu
```sh
sudo add-apt-repository ppa:git-core/ppa -y
sudo apt update
sudo apt upgrade
```
