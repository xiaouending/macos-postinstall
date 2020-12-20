#!/bin/bash

#install xcode
xcode-select --install

# install homebrew
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

# install nvm
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.2/install.sh | bash
nvm install 13
nvm install 10
npm install -g yarn

# install Fira Code font
https://github.com/tonsky/FiraCode

# install main packages
brew install git python

# install cask packages
brew cask install iterm2
brew cask install discord
brew cask install docker
brew cask install google-chrome
brew cask install insomnia
brew cask install telegram
brew cask install visual-studio-code

# vscode settings
{
    "breadcrumbs.enabled": false,
    "editor.fontSize": 16,
    "editor.fontFamily": "Fira Code",
    "editor.fontLigatures": true,
    "editor.fontWeight": "400",
    "editor.tabSize": 2,
    "emmet.showExpandedAbbreviation": "never",
    "editor.minimap.enabled": false,
    "git.enableSmartCommit": true,
    "javascript.updateImportsOnFileMove.enabled": "never",
    "typescript.updateImportsOnFileMove.enabled": "never",
    "window.zoomLevel": 0,
    "workbench.colorTheme": "Monokai Pro (Filter Machine)",
    "workbench.iconTheme": null,
    "workbench.settings.editor": "json",
    "workbench.startupEditor": "newUntitledFile",
    "[javascript]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    },
    "[typescript]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    }
}
