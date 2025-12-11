# Mac OS X Setup

Facing the setup of a new machine (or the need to reinstall after a fresh OS install or the like), here's a very brief and basic list of the usual suspects, related to the setup of a Mac computer to work with (mostly related to a scripting languages context).

## Homebrew & Package Managers

The package manager is the default first thing I always install. Simply following the default steps. Homebrew downloads and installs the Command Line Tools for Xcode, so we're all good. Homebrew Cask is implemented as part of Homebrew now, so we're cask-enabled and ready from the start for our tapping. Finally, `brew-cask-upgrade` provides upgrade-like capabilities to cask, and we're all set.

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
brew tap buo/cask-upgrade
```

If some previously purchased software from the Mac App Store needs to be included, we can use `mas` to ease the installs.

```bash
brew install mas
```

## My curated list of apps (and all that jazz)

Once we have `homebrew`, `cask` (and `mas` if needed) we're ready to go (and yes, these lists might be scripted for some automation to install all, take this as just a curated set):

### Essential Utilities

```bash
# Efficiency booster - install this first!
brew install alfred
```

### Development Environment

#### Terminal & Shell

```bash
# Terminal
brew install iterm2

# Shell & enhancements
brew install zsh zsh-completions zsh-syntax-highlighting zsh-autosuggestions
#Check plugins, templates, themes, etc. at:
#https://github.com/robbyrussell/oh-my-zsh

# Terminal utilities
brew install tree
brew install wget
brew install jq
brew install tldr
brew install thefuck
brew install go2shell
brew install shuttle
```

#### Version Control

```bash
# it GUI tools
brew install sourcetree
brew install tower
brew install rowanj-gitx # Legacy: Still functional but less actively maintained
```

#### Languages & Runtimes

```bash
# Python
brew install python
brew install python3
brew install pyenv
brew install anaconda

# Node.js
brew install node
brew install yarn

# Go
brew install go

# PHP
brew install composer

# Gradle (JVM)
brew install gradle
```

#### IDEs & Editors

```bash
# Modern editors
brew install visual-studio-code

# JetBrains suite
brew install datagrip
brew install intellij-idea
brew install phpstorm
brew install pycharm
brew install rubymine
brew install webstorm

# Other modern editors
brew install sublime-text

# Legacy/Specialized editors
brew install textmate
brew install atom # Legacy: Discontinued by GitHub in 2022, consider VS Code instead
brew install brackets # Legacy: Discontinued by Adobe in 2021
```

#### API & Development Tools

```bash
# API development & testing
brew install rapidapi
brew install postman

# Network & debugging
brew install charles
brew install ngrok

# Documentation
brew install dash

# Utilities
brew install gas-mask
```

#### Databases

```bash
brew install sequel-ace # Modern alternative to sequel-pro
brew install elasticsearch
```

#### DevOps & Infrastructure

```bash
# Cloud & CLI
brew install awscli

# Containers
brew install docker
brew install kitematic

# Infrastructure as Code
brew install vagrant
brew install virtualbox
brew install packer
brew install terraform
brew install vault

# File transfer & storage
brew install cyberduck

# VPN & Security (for dev environment access)
brew install tunnelblick
brew install cloudflare-warp
```

### AI & ML Tools

```bash
# AI Assistants
brew install claude
brew install claude-code
brew install chatgpt
brew install chatgpt-atlas

# AI-Enhanced IDEs
brew install cursor
brew install windsurf

# Local AI models
brew install ollama # Run DeepSeek, Llama, Llava, and other models locally
```

### Browsers

```bash
brew install arc
brew install google-chrome
brew install brave-browser
brew install firefox
```

### Communication & Collaboration

#### Team Collaboration

```bash
# Productivity & boards
brew install slack
brew install microsoft-teams
brew install miro
```

#### Video Conferencing

```bash
brew install zoom
brew install webex
brew install krisp
```

#### Messaging

```bash
brew install telegram
brew install whatsapp
```

#### Social Media

```bash
mas install 409789998 #Twitter
```

### Productivity & Organization

#### Note-taking & documentation

```bash
brew install notion
brew install obsidian
brew install typora
mas install 1091189122 #Bear
brew install evernote
```

#### Utilities

```bash
# Screen capture & annotation
mas install 417602904 #CloudApp
brew install skitch

# System utilities
mas install 937984704 #Amphetamine
brew install bartender
mas install 441258766 #Magnet
```

#### Cloud Storage

```bash
brew install dropbox
brew install google-drive
brew install amazon-photos
brew install synology-drive
```

### Creative & Media

#### Photo & Design

```bash
brew install adobe-creative-cloud
brew install affinity-designer
brew install affinity-photo
brew install gimp
```

#### Reading

```bash
brew install calibre
brew install kindle
```

#### Music & Audio

```bash
brew install spotify
mas install 897118787 #Shazam
```

#### Video

```bash
brew install vlc
```

#### Utilities

```bash
brew install the-unarchiver
```

### Other Applications

```bash
# Blog & web publishing
brew install hugo

# Mapping
brew install google-earth

# Office suite
brew install microsoft-office

# VPN & Privacy (general use)
brew install nordvpn
```

### Xcode

```bash
# Xcode - Will take a long time to download. Only install if needed for iOS/macOS development.
mas install 497799835
```
