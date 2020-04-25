# Installing Node and npm  

Make sure `curl` is installed on your machine:  
`sudo apt install curl`  

## Using a package manager

Per the instructions here:  
https://nodejs.org/en/download/package-manager/#debian-and-ubuntu-based-linux-distributions-enterprise-linux-fedora-and-snap-packages

Navigate to the NodeSource GitHub project for instructions on installing a specific version of Node:  
https://github.com/nodesource/distributions/blob/master/README.md

For Node 12.x, add the NodeSource PPA using the following `curl` command:  
`curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -`

Install Node using the `apt` package manager:  
`sudo apt-get install -y nodejs`  

Check that `node` and `npm` have been installed:  
`node -v`  
`npm -v`

## Using nvm

Install `nvm` using the following command:  
`curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash`

You should have this returned to your terminal:  
```
=> Downloading nvm as script to '/home/[user]/.nvm'

=> Appending nvm source string to /home/[user]/.bashrc
=> Appending bash_completion source string to /home/[user]/.bashrc
=> Close and reopen your terminal to start using nvm or run the following to use it now:

export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion
```

Restart your terminal.  

Install the latest version of `node` and `npm`:  
`nvm install node`  

Check that `node` and `npm` have been installed:  
`node -v`  
`npm -v`  

You can also check the versions you've installed with `nvm` using:  
`nvm list`  