---
title: "Titel"
slug: "slug"
toc: false
image: image.jpg
readingTime: false
date: 2023-01-17, 10:37h
categories: [dev]   

---	

	Homebrew is the easiest and most flexible way to install the UNIX tools
	Apple didn´t include with macOS. It can also install software not
	packaged for your Linux distribution to your home directory without
	requiring sudo.


## Install Homebrew

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```


## Commands

| command                 | description       |
| ----------------------- | ----------------- |
| `brew install git`      | Install a package |
| `brew upgrade git`      |                   |
| `brew unlink git`       |                   |
| `brew link git`         |                   |
| `brew switch git 2.5.0` |                   |
| `brew list --versions git`                        |    List all installed formulae.               |


| flag        | description                                                                                                                                                                                                               |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `-f,  --force` | Install formulae without checking for previously installed keg-only or non-migrated versions. When installing casks, overwrite existing files (binaries and symlinks are excluded, unless originally from the same cask). |
|             |                                                                                                                                                                                                                           |
|             |                                                                                                                                                                                                                           |



