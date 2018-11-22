# Setup your bash terminal

## .bash_profile

- The personal initialization file, executed for login shells
- This script executes when you login
- Stuff you put in there might be your PATH and other important environment variables

**OS X**

The Mac terminal runs the .bash_profile everytime so the entire file difference is irrelevant and using one or both will not do anything different on a mac, so they say.

- http://www.joshstaiger.org/archives/2005/07/bash_profile_vs.html

## Themes

1. Go to [osx terminal themes](https://github.com/lysyi3m/osx-terminal-themes)
1. Clone that repo
2. Go into the repo directory adn double click the desired theme. It will open a new Terminal window with that color scheme.
3. Open Terminal > Preferences > Profiles: Set the theme as the default by clicking the `Default` button at the bottom
4. Quit and relaunch a new bash terminal

## Auto Complete

- Install bash auto complete `curl https://raw.githubusercontent.com/git/git/master/contrib/completion/git-completion.bash -o ~/.git-completion.bash`
- Update your ~/.bash_profile

```bash
# Load git bash completion script
source ~/.git-completion.bash
```

## Git Features

- Run this at your user root: `curl https://raw.githubusercontent.com/git/git/master/contrib/completion/git-prompt.sh -o ~/.git-prompt.sh`
- Add to ~/.bash_profile:

```bash
# Load git bash prompt script
source ~/.git-prompt.sh
```

## Bash Aliases


You can create an alias in your terminal to execute bash commands.  Add any of these to the bottom of your `.bash_profile` and come up with your own ways to be lazy.

Huge thanks to Travis (graywithana) for the idea so long ago to use bash alias for folder navigation!

```bash
# Nav alias
alias jp="cd /Users/jpapaleo/Projects/jordanpapaleo" # This is obvious not going to exist on your computer

# git fetch and git checkout
function gfc() {
    git fetch --prune origin $1;
    git checkout $1;
}

function gnb() {
    git checkout -b $1;
    git push -u origin $1;
}

# Git alias
alias gcm="git checkout master"
alias gcr="git checkout release"
alias gnb=gnb
alias gfc=gfc
alias gcb="git checkout $1"
alias gma="git merge abort"
alias gmm="git merge master"
alias gpom="git push origin master" # dont judge me
alias gpro="git pull --rebase origin master"
alias gpru="git pull --rebase upstream master"
alias gra="git rebase --abort"
alias grc="git rebase --continue"

# Node/NPM alias
alias cra="create-react-app"
alias purge="rm -rf node_modules package-lock.json; npm i"
alias dev="npm run dev"
alias devs="npm run dev:s"

# System alias
alias bb='/bin/bash'
alias hideFiles='defaults write com.apple.finder AppleShowAllFiles NO; killall Finder /System/Library/CoreServices/Finder.app'
alias showFiles='defaults write com.apple.finder AppleShowAllFiles YES; killall Finder /System/Library/CoreServices/Finder.app'
```

