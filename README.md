This is [Berkeley's](https://github.com/BerkeleyTrue/zmk-keyboards) ZMK firmware configuration. It consists of a 36-keys base layout for my 5-column wireless Corne  

## Generate layout with keymap-drawer
Install keymap-drawer:
```bash
brew install pipx
pipx ensurepath
pipx install keymap-drawer
```

Generate new svg:
```bash
keymap -c generate-keymap-svg/corne.keymap.config.yaml parse -z ./config/corne.keymap > generate-keymap-svg/corne.keymap.yaml && keymap -c generate-keymap-svg/corne.keymap.config.yaml draw generate-keymap-svg/corne.keymap.yaml > ./assets/corne.svg
```

![](assets/corne.svg)