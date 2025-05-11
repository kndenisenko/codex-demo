---
title: 'Пример файла, скопированного из Obsidian'
author: 'ZX'
---

# Пример файла, скопированного из Obsidian.


#linux
Базовые команды при установке нового инстанса WSL или для ручного запуска на сервере
## Fedora
```sh
sudo dnf update
sudo dnf install mc htop make curl wget ncdu vim ca-certificates tmux git bat zsh
```
## Debian / Ubuntu
```sh
sudo apt update
sudo apt install install mc htop make curl wget ncdu vim ca-certificates tmux git bat zsh
```

## Ручная установка OMZ и плагинов
Установка OMZ
`sh -c "$(wget https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh -O -)"`

Плагин zsh-autosuggestions
`git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions`

Плагин zsh-syntax-highlighting
`git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting`

Скопировать в .zshrc
```sh
plugins=(
	git
	zsh-autosuggestions	
	zsh-syntax-highlighting
)
```
