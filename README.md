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
git submodule add https://github.com/kraxli/astronvim_lua_user.git ~/.config/astronvim/lua/user

# windows:
git clone --recurse-submodules https://github.com/kraxli/astronvim $APPDATA$\Local\astronvim
# git submodule add https://github.com/kraxli/astronvim_lua_user.git $APPDATA$\Local\astronvim\lua\user
# Windows Powershell:
git clone --recurse-submodules https://github.com/kraxli/astronvim ~\AppData\Local\astronvim
# git submodule add https://github.com/kraxli/astronvim_lua_user.git ~\AppData\Local\astronvim\lua\user
```

## Initialize AstroVim

```sh
nvim --headless -c 'autocmd User PackerComplete quitall' -c 'PackerSync'
```

## Further setups and installations from within Nvim

see [Setups in astronivim/github.io](https://astronvim.github.io/#-setup)
