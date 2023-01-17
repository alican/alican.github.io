---
title: "Setup your macOS Terminal Warp+Starship+Zsh"
slug: "setup-your-macos-terminal-warp-starship-zsh"
toc: false
image: image.jpg
readingTime: false
date: 2023-01-17, 10:43h
categories: [dev]   

---	

## Homebrew installieren

[Starship](https://starship.rs/) ist ein Shell-Prompt der in Rust geschrieben ist, super schnell ist und für macOS, Windows und Linux verfügbar ist.

## Starship installieren

Install the latest version for your system:

```bash
curl -sS https://starship.rs/install.sh | sh
```

oder 

```bash
brew install starship
```


## Oh-my-zsh

Oh My Zsh is an open source, community-driven framework for managing your [zsh](https://www.zsh.org/) configuration.

### Installation

```bash
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```


```ad-important
**_NOTE: elements in zsh arrays are separated by whitespace (spaces, tabs, newlines...). DO NOT use commas._**
```

List of plugins:

https://github.com/ohmyzsh/ohmyzsh/wiki/Plugins-Overview


## Add environment path in zsh


```bash
# append
path+=('/Applications/Visual\ Studio\ Code.app/Contents/Resources/app/bin')
# or prepend
path=('/Applications/Visual\ Studio\ Code.app/Contents/Resources/app/bin' $path)
# export to sub-processes (make it inherited by child processes)
export PATH
```