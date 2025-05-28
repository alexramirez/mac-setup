# Mac OS X setup
Facing the setup of a new machine (or the need to reinstall after a fresh OS install or the like), here's a very brief and basic list of the usual suspects, related to the setup of a mac computer to work with (mostly related to a scripting languages context).

## Homebrew & Cask
The package manager is the default first thing I always install. Simply following the default steps. Homebrew downloads and installs the Command Line Tools for Xcode, so we're all good. Homebrew Cask is implemented as part of Homebrew now, so we're cask-enabled and ready from the start for our tapping. Finally, `brew-cask-upgrade` provides upgrade-like capabilities to cask, and we're all set.
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
brew tap buo/cask-upgrade
```
## Mac App Store
If some previously purchased software from the Mac App Store needs to be included, we can use `mas` to ease the installs.

```bash
brew install mas
```

## My curated list of apps (and all that jazz)
Once we have `homebrew`, `cask` (and `mas` if needed) we're ready to go (and yes, these lists might be scripted for some automation to install all, take this as just a curated set):

### Productivity

```bash
# Efficiency booster
brew install alfred

# CloudApp
mas install 417602904

# Slack
brew install slack

# Miro
brew install miro

# Notes & related
mas install 1091189122 #Bear
brew install evernote
brew install notion
brew install obsidian
brew install skitch
brew install typora

# Amphetamine
mas install 937984704

# Bartender
brew install bartender

# Magnet
mas install 441258766
```

### Browsers

```bash
# Browsers
brew install arc
brew install google-chrome
brew install brave-browser
brew install firefox
```

### AI tools

```bash
# Anthropic
brew install claude

# OpenAI
brew install chatgpt

# IDEs
brew install cursor
brew install windsurf

# Other models/tools
brew install ollama # DeepSeek, Llama,Llava, etc.
```

### Common apps

```bash

# Calibre
brew install calibre

# Blog
brew install hugo

# Personal cloud storage
brew install amazon-photos
brew install dropbox

# Gimp
brew install gimp

# Some of the Google stuff
brew install google-drive
brew install google-earth

# Kindle
brew install kindle

# MS
brew install microsoft-office

# Photo editing
brew install adobe-creative-cloud
brew install affinity-designer
brew install affinity-photo

# Spotify
brew install spotify

# Shazam
mas install 897118787

# Twitter
mas install 409789998

# The Unarchiver
brew install the-unarchiver

# VLC
brew install vlc

# Videoconference
brew install microsoft-teams
brew install webex
brew install zoom
brew install krisp

# Messaging
brew install telegram
brew install whatsapp
```

### Development

```bash
# A good terminal
brew install iterm2
brew install jq
brew install zsh zsh-completions zsh-syntax-highlighting zsh-autosuggestions
# And definitely check plugins, templates, themes, etc. at:
# https://github.com/robbyrussell/oh-my-zsh
brew install tree
brew install wget
brew install tldr
brew install thefuck

# Go2Shell
brew install go2shell

# Shuttle
brew install shuttle 

# AWS CLI
brew install awscli

# API development
brew install rapidapi
brew install postman

# Text editors/IDEs
brew install textmate
brew install sublime-text
brew install brackets
brew install atom
brew install visual-studio-code

# Charles proxy
brew install charles

# Dash
brew install dash

# Docker
brew install docker
brew install kitematic

# ES
brew install elasticsearch

# Gas Mask
brew install gas-mask

# Git-related
brew install rowanj-gitx
brew install sourcetree
brew install tower

# Gradle
brew install gradle

# GoLang
brew install go

# JS
brew install node
brew install yarn

# Ngrok
brew install ngrok

# Python
brew install python
brew install python3
brew install pyenv
brew install anaconda

# DevOps
brew install vagrant
brew install virtualbox
brew install packer
brew install terraform
brew install vault

# Cloud storage and related
brew install cyberduck

# JetBrains
brew install phpstorm
brew install pycharm
brew install rubymine
brew install intellij-idea
brew install webstorm

# PHP & related
brew install composer

# Databases
brew install sequel-ace # Alternative to sequel-pro 

# VPN
brew install nordvpn
brew install tunnelblick
brew install cloudflare-warp

# Xcode. Will take forever to download, yes. Not needed by everyone.
mas install 497799835
```
