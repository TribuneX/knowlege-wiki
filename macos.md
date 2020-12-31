---
description: Everything I need to know about macOS and my used apps on this platform.
---

# macOS

## Dotfiles

I try to keep all of my configuration for cli tools and apps in [structured dotfiles](https://github.com/tribunex/dotfiles). Setting up a new Mac is easy and can be done within an hour.

## Homebrew

I install all non-appstore apps and cli-tools using [Homebrew](https://brew.sh). Homebrew especially shines when I need to setup a new mac. Homebrew has a nice feature called [Homebrew bundle](https://github.com/Homebrew/homebrew-bundle), which allows to keep track of all installed apps in a Brewfile. This files includes all cli-tools installed by Homebrew, all non-appstore apps installed by [Homebrew cask](https://github.com/Homebrew/homebrew-cask) and even all app-store apps installed by [mas-cli](https://github.com/mas-cli/mas).

After installing a new software via brew or the AppStore, I need to update my Brewfile with the following command:

    brew bundle dump --force

## Zsh

I use zsh as my main shell (before Apple changed the default shell from bash to zhs). I started customizing my zsh shell with the [oh-my-zsh](https://github.com/ohmyzsh/ohmyzsh), but quickly discovered that my shell was getting slower and slower. Sometimes, the shell needed multiple seconds to start!

Therefore, I looked for some speed improvements and ended up using [zinit](https://github.com/zdharma/zinit). It makes your shell startup time alot quicker, however I found it really difficult to configure. I had a working .zshrc config, but I did not understand every command in detail.

I am currently using [Antibody](https://github.com/getantibody/antibody) as my zsh plugin manager (inspired by the dotfiles from [Nikita](https://github.com/nikitavoloboev/dotfiles). It is a lot easier to use, as it requires only a simple txt file with the [plugins](https://github.com/TribuneX/dotfiles/blob/master/zsh/.plugins.txt) I want to use.

The plugins must be translated into a static file, which will then be loaded at every startup:

    antibody bundle < ~/dotifiles/zsh/.plugins.txt > ~/dotifiles/zsh/.plugins.sh

 

