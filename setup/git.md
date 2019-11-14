# Git Setup

Get latest version of git: `https://git-scm.com/download/mac`

# Global config

Create a global config to associate your commits to you.

```bash
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
```

## Global ignore

There are certain files created by particular editors, IDEs, operating systems, etc., that do not belong in a repository. But adding system-specific files to the repo's .gitignore is considered a poor practice. This file should only exclude files and directories that are a part of the package that should not be versioned.

*See https://help.github.com/ignore-files/ for more about ignoring files.*

```bash
touch ~/.gitignore
git config --global core.excludesfile ~/.gitignore
```

Add the following to your `.gitignore`

```bash
# Node
npm-debug.log
/node_modules

# Mac
.DS_Store

# Visual Code
.history
.vscode

# WebStorm
.idea/

# vi
*~

# General
npm-debug.log*
yarn-debug.log*
yarn-error.log*
log/
*.log
*.dump

# Testing
/coverage

```
