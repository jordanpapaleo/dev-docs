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
