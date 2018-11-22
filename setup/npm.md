# Npm Setup

Follow the steps below to create your account and setup the auth token.

1. Navigate to the [npm](http://www.npmjs.com) site and create an account.
1. Open your 'Profile Settings' page and click on the 'Tokens' tab.
1. Create a 'read and publish' token.
1. Open `~/.npmrc` in your favorite editor.  If you don't have this file, create it.
1. Add `//registry.npmjs.org/:_authToken=YOUR_TOKEN_HERE` to the top of the file.
1. Open `~/.bash_profile` in your favorite editor.  If you don't have this file, create it.
1. Add: **This code must go ABOVE your `NVM_DIR` export.**

```bash
# Set npm auth token for installing private packages
export NPM_TOKEN="YOUR_TOKEN_HERE"
```
