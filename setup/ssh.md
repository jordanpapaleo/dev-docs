# SSH Keys Setup

We use SSH (Secure SHell) keys to interact with our code repositories.  To do this you will need to copy the content of a key on your computer and add it to our repo providers: Github or Bitbucket.  You may already have a key on your computer that you can use.

**Check for a key:** `cat ~/.ssh/id_rsa.pub` You can skip to copy key if you have one

**Create a new key if needed:** `ssh-keygen -t rsa -b 2048`

**Verify new key:** `cat ~/.ssh/id_rsa.pub`

**Copy key:** `cat ~/.ssh/id_rsa.pub | pbcopy`

**Add your key:** Both Github and Bitbucket provide an interface for this on their websites

**Test your keys:** `ssh -T git@github.com` `ssh -T git@bitbucket.org`
