---
title: "Git"
slug: "git"
toc: true
image: git.png
readingTime: false
date: 2022-10-17T22:48:08+02:00
categories: [cheatsheet, dev]   

---

## Install Git
### Install Git on macOS

Install Git using Homebrew:

```bash 
    brew install git
```

Verify the installation was successful:

```bash
    git --version
```

### Configure your Git username and email 

```bash

```

```bash 
    git config --global user.email "git@mail"
    git config --global user.name "Alican Toprak
```


### Install git-credential-osxkeychain
 
```bash 
    git credential-osxkeychain 
```

### Representation

Draw a text-based graphical representation of the commit history on the left hand side of the output.

```bash
    git log --all --decorate --oneline --graph
```