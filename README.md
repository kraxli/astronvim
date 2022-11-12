# AstroNvim User Configuration

My personal user config for AstroVim

## Installation

### Linux

```sh
  git clone https://github.com/AstroNvim/AstroNvim.git ~/.config/nvim
  git clone --recurse-submodules https://github.com/kraxli/astronvim ~/.config/astronvim
  git submodule add <your local repo> ~/.config/astronvim/lua/local
  git clone https://github.com/kraxli/astronvim_lua_user2.git ~/.config/astronvim/lua/user
```

<!-- # windows: -->
<!-- git clone --recurse-submodules https://github.com/kraxli/astronvim $APPDATA$\Local\astronvim -->
<!-- git submodule add <your local repo> $APPDATA$\Local\astronvim\lua\local -->

### Windows Powershell

In case you are using `nvim` on locked down machine, but you have (a) free location(s) on your drive, so you can change the workding directories.

Most importantly set `XDG_DATA_HOME` as environmental (user) variable. E.g. `XDG_DATA_HOME=C:\SRDEV\config`.
You can also the location of the configuration location of `nvim` and `astronvim` by setting `XDG_CONFIG_HOME` in your (user) environmental variables. E.g. `XDG_CONFIG_HOME=C:\SRDEV\config`. In case you set `XDG_CONFIG_HOME` you need to replace `$env:LOCALAPPDATA` below by `$env:XDG_CONFIG_HOME`.

#### make back up

```sh
 Move-Item $env:LOCALAPPDATA\nvim $env:LOCALAPPDATA\nvim.bak
 Move-Item $env:LOCALAPPDATA\astronvim $env:LOCALAPPDATA\astronvim.bak
```

#### Clean old plugins

```sh
  Move-Item $env:LOCALAPPDATA\nvim-data $env:LOCALAPPDATA\nvim-data.bak
```

#### Clone the repo

```sh
  git clone https://github.com/AstroNvim/AstroNvim $env:LOCALAPPDATA\nvim
  git clone --recurse-submodules https://github.com/kraxli/astronvim $env:LOCALAPPDATA\astronvim
  git clone https://github.com/kraxli/astronvim_lua_user2.git $env:LOCALAPPDATA\astronvim\lua\user
```

### Initialize AstroVim

```sh
nvim --headless -c 'autocmd User PackerComplete quitall' -c 'PackerSync'
```

## Further setups and installations from within Nvim

see [Setups in astronivim/github.io](https://astronvim.github.io/#-setup)
