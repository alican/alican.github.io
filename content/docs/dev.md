# Dev


## Setup macOS for development

### Install Homebrew

Paste this line in your macOS Terminal: ```/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"```

Brew Manpage:
https://docs.brew.sh/Manpage


## Python

### Install python3 on macOS



## SSH

Generate a Private/Pub-Key with et25519 and a Comment.

```ssh-keygen -t ed25519 -f ~/.ssh/alican.ed25519 -C "Key for my homeserver"```

Transfer the pub key to remote host. Typicall its located at ```/home/$USERNAME/.ssh/```

```ssh-copy-id -i ~/.ssh/alican.ed25519.pub alican@example.com```

Login SSH with an explicit key
ssh -i ~/.ssh/alican.ed25519 alican@example.com

Deaktivate password authentication. 
Open the config ```/etc/ssh/sshd_config``` and edit following lines like this:

```
PasswordAuthentication no
ChallengeResponseAuthentication no
```
Restart the SSH server to apply the changes

```systemctl restart ssh```


