# Dev Laptop Setup

1. [Setup bash](bash.md)
1. [Setup Homebrew](homebrew.md)
1. [Setup NVM or Node](node.md)

## Dev Environment

1. Install IDE of choice
1. [Setup git](git.md)
1. [Setup npm](npm.md)
1. [Setup SSH](ssh.md)
1. [Setup VM](vm.md)

## Extras

1. Install [f.lux](https://justgetflux.com/) to make you life better
1. Setup finder to have markdown preview
    - Download the latest [release](https://github.com/downloads/toland/qlmarkdown/QLMarkdown-1.2.1.zip)
    - Extract it somewhere temporarily, go into the extracted directory
    - Copy the QLMarkdown.qlgenerator file into ~/Library/QuickLook
        - `mv QLMarkdown.qlgenerator/ ~/Library/QuickLook`
        - you may need to create this directory `mkdir ~/Library/QuickLook`
    - Relaunch Finder by alt+right-clicking on the icon in the dock and selecting the option at the bottom.
1. Fix Home and End Keys

```bash
mkdir -p ~/Library/KeyBindings
vi ~/Library/KeyBindings/DefaultKeyBinding.dict

{
"\UF729"  = "moveToBeginningOfLine:";
"\UF72B"  = "moveToEndOfLine:";
"$\UF729" = "moveToBeginningOfLineAndModifySelection:";
"$\UF72B" = "moveToEndOfLineAndModifySelection:";
}
```
