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

# Wunderlist
mas install 410628904

# Notes & skitch
brew cask install evernote
brew cask install skitch

# Amphetamine
mas install 937984704

# Magnet
mas install 441258766
```

### Common apps

```bash
# Default browser. I like Chrome.
brew cask install google-chrome

# Calibre
brew cask install calibre

# Dropbox
brew cask install dropbox

# Firefox
brew cask install firefox

# Gimp
brew cask install gimp

# Some of the Google stuff
brew cask install google-photos-backup
brew cask install google-earth

# Kindle
brew cask install kindle

# Spotify
brew cask install spotify

# Shazam
mas install 897118787

# Skype
brew cask install skype

# Twitter
mas install 409789998

# The Unarchiver
brew cask install the-unarchiver

# Whatsapp
brew cask install whatsapp

# VLC
brew cask install vlc
```

### Development

```bash
# A good terminal
brew cask install iterm2
brew install jq
brew install zsh zsh-completions 
# And definitely check plugins, templates, themes, etc. at:
# https://github.com/robbyrussell/oh-my-zsh

# AWS CLI
brew install awscli

# A good text editor / text IDE
brew cask install textmate
brew cask install sublime-text
brew cask install brackets
brew cask install atom

# Charles
brew cask install charles

# Docker
brew cask install docker
brew cask install kitematic

# Gas Mask
brew cask install gas-mask

# Git-related
brew cask install rowanj-gitx
brew cask install sourcetree
brew cask instal kdiff3

# GoLang
brew install go

# Ngrok
brew cask install ngrok

# Python
brew install python
brew install python3

# Vagrant
brew cask install vagrant

# Packer
brew install packer

# FTP & related
brew cask install cyberduck
brew cask install filezilla

# JetBrains
brew cask install phpstorm
brew cask install pycharm
brew cask install rubymine
brew cask install intellij-idea

# PHP & related
brew install homebrew/php/composer

# Sequel Pro
brew cask install sequel-pro

# Terrafom
brew install terraform

# Xcode. Will take forever to download, yes. Not needed by everyone.
mas install 497799835
```

## Google Chrome stuff

Some useful pointers if we have not added those to the Google account yet

- https://chrome.google.com/webstore/detail/authy/gaedmjdfmmahhbjefcbgaolhhanlaolb
- https://chrome.google.com/webstore/detail/postman/fhbjgbiflinjbdggehcddcbncdddomop
- https://chrome.google.com/webstore/detail/browserstack-local/mfiddfehmfdojjfdpfngagldgaaafcfo
- https://chrome.google.com/webstore/detail/json-editor/lhkmoheomjbkfloacpgllgjcamhihfaj
- https://chrome.google.com/webstore/detail/google-keep-notes-and-lis/hmjkmjkepdijhoojdojkdfohbdgmmhki
- https://chrome.google.com/webstore/detail/google-hangouts/knipolnnllmklapflnccelgolnpehhpl


## Others/ToDo

```
# Wine, winebottler
```
