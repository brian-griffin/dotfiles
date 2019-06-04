# My Dotfiles

A place to store my dot files (desperately needs an update!)

## Usage

Clone into ~/dotfiles/
```bash
git clone git@github.com:brian-griffin/dotfiles.git ~/dotfiles
```

Then add symlinks in your ~/ directory
```bash
ln -nfs ~/dotfiles/vim/ .vim
ln -nfs ~/dotfiles/vimrc .vimrc
ln -nfs ~/dotfiles/bash_profile .bash_profile
ln -nfs ~/dotfiles/bash_aliases .bash_aliases
ln -nfs ~/dotfiles/gitconfig .gitconfig
```

Fetch submodules after cloning repo, in ~/dotfiles
```bash
git submodule update --init
```

## Maintenance

Removing submodules
```bash
cd ~/dotfiles
git submodule deinit vim/bundle/[MODULE-NAME]
git rm -r vim/bundle/[MODULE-NAME]
```

Adding new submodules
```bash
cd ~/dotfiles
git submodule add [MODULE-GIT-URL] vim/bundle/[MODULE-NAME]
```
