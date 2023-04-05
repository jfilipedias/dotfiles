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
ln -s ~/.dotfiles/.config.fish ~/.config/fish/config.fish
```


## Setups

### Shell
Install fish on Ubuntu: 
```sh
sudo apt install fish
chsh -s $(which fish)
```

Install zsh on Fedora: 
```sh
sudo dnf install zsh
sudo dnf install utils-linux-user
chsh -s $(which fish)
```

Install starship:
```sh
curl -sS https://starship.rs/install.sh | sh
```
### Node

Install fnm:
```sh
curl -fsSL https://fnm.vercel.app/install | bash
```

Install latest stable version of node:
```sh
fnm install --lts
```

Install pnpm:
```sh
curl -fsSL https://get.pnpm.io/install.sh | sh -
```

Install yarn:
```sh
npm install -g yarn
```


### Fira Code
Install on Ubuntu:
```sh
sudo apt install fonts-firacode
```

Install on fedora:
```sh
sudo dnf install fira-code-fonts
```

### Git

Updates git on Ubuntu
```sh
sudo add-apt-repository ppa:git-core/ppa -y
sudo apt update
sudo apt upgrade
```
