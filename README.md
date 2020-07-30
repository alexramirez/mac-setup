# Mac OS X setup
Facing the setup of a new machine (or the need to reinstall after a fresh OS install or the like), here's a very brief and basic list of the usual suspects, related to the setup of a mac computer to work with (mostly related to a scripting languages context).

## Homebrew & cask
The package manager is the default first thing I always install. Simply following the default steps. Homebrew downloads and installs the Command Line Tools for Xcode, so we're all good. `brew cask` handles the tapping, so we are cask-enabled too. Finally, `brew-cask-upgrade` provides upgrade-like capabilities to cask, and we're all set.
```bash
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
brew cask
brew tap buo/cask-upgrade
```
## Mac App Store
If some previously purchased software from the Mac App Store needs to be included, we can use `mas` to ease the installs.

```bash
brew install mas
```

## My curated list of apps (and all that jazz)
Once we have `homebrew`, `cask` (and `mas` if needed) we're ready to go (yes, these lists might be scripted, this is just a curated set):

### Productivity

```bash
# Efficiency booster
brew cask install alfred

# CloudApp
mas install 417602904

# Slack
brew cask install slack

# Notes & related
brew cask install evernote
brew cask install skitch
mas install 1091189122 #Bear

# Amphetamine
mas install 937984704

# Bartender
brew cask install bartender

# Magnet
mas install 441258766
```
### Browsers

```bash
# Browsers
brew cask install google-chrome
brew cask install brave-browser
brew cask install firefox
```

### Common apps

```bash

# Authy
brew cask install authy

# Calibre
brew cask install calibre

# Personal cloud storage
brew cask install amazon-photos
brew cask install dropbox

# Gimp
brew cask install gimp

# Some of the Google stuff
brew cask install google-photos-backup-and-sync
brew cask install google-earth

# Kindle
brew cask install kindle

# MS
brew cask install microsoft-office

# Spotify
brew cask install spotify

# Shazam
mas install 897118787

# Twitter
mas install 409789998

# The Unarchiver
brew cask install the-unarchiver

# VLC
brew cask install vlc

# Videoconference
brew cask install skype
brew cask install skype-for-business
brew cask install zoomus

# Messaging
brew cask install telegram
brew cask install whatsapp
```

### Development

```bash
# A good terminal
brew cask install iterm2
brew install jq
brew install zsh zsh-completions zsh-syntax-highlighting zsh-autosuggestions
# And definitely check plugins, templates, themes, etc. at:
# https://github.com/robbyrussell/oh-my-zsh
brew install tree
brew install wget
brew install tldr
brew install thefuck

# Go2Shell
brew cask install go2shell

# Shuttle
brew cask install shuttle 

# AWS CLI
brew install awscli

# API development
brew cask install paw
brew cask install postman

# Text editors/IDEs
brew cask install textmate
brew cask install sublime-text
brew cask install brackets
brew cask install atom
brew cask install visual-studio-code

# Charles proxy
brew cask install charles

# Dash
brew cask install dash

# Docker
brew cask install docker
brew cask install kitematic

# ES
brew install elasticsearch

# Gas Mask
brew cask install gas-mask

# Git-related
brew cask install rowanj-gitx
brew cask install sourcetree
brew cask install tower

# Gradle
brew install gradle

# GoLang
brew install go

# Ngrok
brew cask install ngrok

# Python
brew install python
brew install python3
brew cask install anaconda

# DevOps
brew cask install vagrant
brew cask install virtualbox
brew install packer
brew install terraform
brew install vault

# Cloud storage and related
brew cask install cyberduck

# JetBrains
brew cask install phpstorm
brew cask install pycharm
brew cask install rubymine
brew cask install intellij-idea

# PHP & related
brew install composer

# Databases
brew cask install sequel-pro

# VPN
brew cask install tunnelblick

# Xcode. Will take forever to download, yes. Not needed by everyone.
mas install 497799835
```

## Google Chrome stuff

Some useful pointers if we have not added those to the Google account yet

- https://chrome.google.com/webstore/detail/authy/gaedmjdfmmahhbjefcbgaolhhanlaolb
- https://chrome.google.com/webstore/detail/browserstack-local/mfiddfehmfdojjfdpfngagldgaaafcfo
- https://chrome.google.com/webstore/detail/json-editor/lhkmoheomjbkfloacpgllgjcamhihfaj
- https://chrome.google.com/webstore/detail/google-keep-notes-and-lis/hmjkmjkepdijhoojdojkdfohbdgmmhki
- https://chrome.google.com/webstore/detail/google-hangouts/knipolnnllmklapflnccelgolnpehhpl


## Others/ToDo

```
# Wine, winebottler
```
