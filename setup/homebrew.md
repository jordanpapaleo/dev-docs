# Homebrew installation

[instructions](http://coolestguidesontheplanet.com/installing-homebrew-os-x-yosemite-10-10-package-manager-unix-apps/)

1. Required for homebrew: Install Xcode command line tools

```bash
sudo xcodebuild -license
xcode-select --install
```

1. Install homebrew

```bash
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
brew doctor
```

1. [Setup git bash completion](https://github.com/bobthecow/git-flow-completion/wiki/Install-Bash-git-completion)

```bash
brew install git bash-completion
```

Add `[ -f /usr/local/etc/bash_completion ] && . /usr/local/etc/bash_completion` to `~./bash_profile`
