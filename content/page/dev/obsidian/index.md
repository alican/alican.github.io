---
title: "Obsidian"
slug: "obsidian"
toc: true
image: obsidian.jpg
readingTime: false
date: 2023-01-11T22:48:08+02:00
categories: [cheatsheet, dev]   

---


## Mobile App (iOS/Android) synchronization with git


You don't need the premium sync function of the app or another app like a git client to backup and sync- your fault. The Obsidian Git plugin is also available for mobile and gives everything you need to synchronize your Obsidian fault between different mobile and desktop devices.

### Install Obsidian Mobile
- [Obsidian for iOS](https://apps.apple.com/us/app/obsidian-connected-notes/id1557175442)
- [Obsidian for Android](https://play.google.com/store/apps/details?id=md.obsidian)


## Create a git repository (on github.com for example)

1. Create an empty repository
2. Create a new access token [(Settings->Developer Settings->Tokens)](https://github.com/settings/tokens) with the Repo scope and copy the token

### Configure Obsidian

1. Create a new vault in your mobile obsidian app
2. Enter into the new vault
3. Got the Settings->About->Advanced and override the config folder to `.obsidian.mobile` for example. This avoids misconfigurations when you use the desktop client because some settings and plugins are different on mobile and desktop. You have  than two config folders in your Vault.
4. Activate Community Plugins and install the Obsidian-Git. 
5. Enable the Obsidian-Git plugin and go to the plugin settings
6. Enter in the username field `__token__` (two underscore)
7. Enter the created github personal access token in the password field
8. Close the Settings and open the _command pallete_. Enter `Clone an existing remote repo`. It will recommended if you type the first words.
9. Enter the Repository URL of your Git-Repository. I recommend *https* and not ssh.
10. Leave path field empty. And choose that their is no obsidian config folder in the remote vault. 
11. Restart the app.


