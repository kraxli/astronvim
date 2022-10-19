# AstroNvim User Configuration

My personal user config for AstroVim

## Installation

### AstroNvim

```sh
git clone https://github.com/AstroNvim/AstroNvim.git ~/.config/nvim
```

### User settings

```sh
# Linux:

git clone --recurse-submodules https://github.com/kraxli/astronvim ~/.config/astronvim
git submodule add <your local repo> ~/.config/astronvim/lua/local

# windows:
git clone --recurse-submodules https://github.com/kraxli/astronvim $APPDATA$\Local\astronvim
git submodule add <your local repo> $APPDATA$\Local\astronvim\lua\local

# Windows Powershell:
git clone --recurse-submodules https://github.com/kraxli/astronvim ~\AppData\Local\astronvim
git submodule add <your local repo> ~\AppData\Local\astronvim\lua\local
```

## Initialize AstroVim

```sh
nvim --headless -c 'autocmd User PackerComplete quitall' -c 'PackerSync'
```

## Further setups and installations from within Nvim

see [Setups in astronivim/github.io](https://astronvim.github.io/#-setup)
