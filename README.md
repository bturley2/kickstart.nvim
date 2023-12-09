# bturley2's kickstart.nvim

This repo is based off of the [kickstart.nvim](https://github.com/nvim-lua/kickstart.nvim) repo. It already contains a number of critical basic plugins such as treesitter for basic linting, Mason to quickly install language support, fzf and more.

Default font is set to `catppuccin-macchiato` theme, but you're welcome to change it. All configurations are in the `~/.config/nvim/init.lua` file.

The [lazy.nvim](https://github.com/folke/lazy.nvim) plugin manager is already installed to make future plugins easier to add.

## Custom Install Steps 

Install what's in this repo with:
```
git clone https://github.com/bturley2/kickstart.nvim.git "${XDG_CONFIG_HOME:-$HOME/.config}"/nvim
```


Before anything else, use Mason extension to install autocomplete for whatever languages you plan to use:
```
# to list options
:Mason

# some examples you may wish to install for go, python, or rust autocomplete
:MasonInstall gopls goimports pylint rust-analyzer
```

## Tips

Many useful plugins are already installed such as [comment.nvim](https://github.com/numToStr/Comment.nvim) which allows you to toggle comments in code using
```
# in regular mode
gcc

# in visual mode
gc
```


Or [nvim-cmp](https://github.com/hrsh7th/nvim-cmp) which provides autocomplete. Detailed keybindings for this can be found here: https://linovox.com/install-and-use-nvim-cmp/ 
With the key ones being:
```
C-Space -> Opens Menu
C-e     -> Closes Menu
```

## etc

And with that, you should have a working Neovim editor! 

For more details instructions, or more information on the installed plugins, check out the base Kickstart.nvim project repo: https://github.com/nvim-lua/kickstart.nvim

