An icon theme (do nothing about colors) for [xplr](https://github.com/sayanarijit/xplr).

Based on [nvim-web-devicons](https://github.com/kyazdani42/nvim-web-devicons) with some input from [nnn](https://github.com/jarun/nnn). Text formats are well covered. Binary formats still needs some attention.

## Requirements

- [A patched font](https://www.nerdfonts.com/)

## Installation

### Install manually

- Add the following line in `~/.config/xplr/init.lua`

  ```lua
  local home = os.getenv("HOME")
  package.path = home
  .. "/.config/xplr/plugins/?/init.lua;"
  .. home
  .. "/.config/xplr/plugins/?.lua;"
  .. package.path
  ```

- Clone the plugin

  ```bash
  mkdir -p ~/.config/xplr/plugins

  git clone https://github.com/prncss-xyz/icons.xplr ~/.config/xplr/plugins/icons
  ```

- Require the module in `~/.config/xplr/init.lua`

  ```lua
  require"icons".setup()
  ```
