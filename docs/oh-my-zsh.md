# Installing oh-my-zsh  

Install `curl` and `zsh`:  

`sudo apt install curl`  
`sudo apt install zsh`  

Install `oh-my-zsh`:  
`sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`  

If `nvm` was installed using `bash`, check the `~/.zshrc` file and make sure the following is included so `nvm` paths are also set up with `zsh`:  

```
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion
```