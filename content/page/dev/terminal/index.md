---
title: "Titel"
slug: "slug"
toc: false
image: terminal.jpg
readingTime: false
date: 2023-01-17, 10:29h
categories: [dev, terminal]   

---	



# SSH

Generate a Private/Pub-Key with et25519 and a Comment.

```ssh-keygen -t ed25519 -f ~/.ssh/alican.ed25519 -C "Key for my homeserver"```

Transfer the pub key to remote host. Typicall its located at ```/home/$USERNAME/.ssh/```

```ssh-copy-id -i ~/.ssh/alican.ed25519.pub alican@example.com```

If you the ssh keys manually, be sure that the files have the correct permissions:

```
chmod 700 .ssh
chmod 600 ~/.ssh/authorized_keys
```

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

Save remote Hosts on your local client at  ```~/.ssh/config```

```
Host alican.de
     HostName alican.de
     User alican
     IdentityFile ~/.ssh/alican.ed25519

Host klipper
     HostName 192.168.178.42
     User pi
     Port 2000
     LocalForward 80 localhost:8080
     IdentityFile ~/.ssh/klipper.ed25519
     
```

Now just run the ssh command like this

``` ssh alican.de```


