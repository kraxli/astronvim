# Fixes and Workarounds

## ekickx/clipboard-image.nvim

Health issue: https://github.com/ekickx/clipboard-image.nvim/issues/50

## iamcco/markdown-preview.nvim",

tslib not found:

```zsh
    # with npm:
    cd $XDG_DATA_HOME/nvim/lazy/markdown-preview.nvim/app && npm install && npm audit fix --force

    # or with yarn:
   cd $XDG_DATA_HOME/nvim/lazy/markdown-preview.nvim/app && yarn install
```
