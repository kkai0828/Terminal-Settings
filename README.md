# Terminal-Settings
oh-my-zsh + powerlevel10k and some plugins

# Install zsh and iTerm2
```shell
    $ brew install zsh # mac  
    $ brew install --cask iterm2
```
```
    $ sudo sh -c "echo $(which zsh) >> /etc/shells"  # 將 zsh 加入系統的 shell 清單，需要輸入管理者密碼
    $ chsh -s $(which zsh) # 把 zsh 設為預設 shell
```

# Install oh-my-zsh
```shell
    # via curl
    $ sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

    # via wget
    $ sh -c "$(wget https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh -O -)"
```

# Install powerlevel10k
```shell
   $ git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k 
```
# Change zsh Theme to powerlevel10k
```shell
    $ vi ~/.zshrc
    # Find ZSH_THEME and Change to 
    ZSH_THEME="powerlevel10k/powerlevel10k"
```
Then follow the p10k configuration wizard, if it doesn't show up.
```
    $ p10k configure
```
[configuration guide](https://www.onejar99.com/terminal-iterm2-zsh-powerlevel10k/)
# p10k Settings
```
    $ vi ~/.p10k.zsh
```
[guide](https://onejar99.com/zsh-powerlevel10k-custom-config-note/#more-1016)
  
# Plugins  
```
    # zsh-autosuggestions
    $ git clone git://github.com/zsh-users/zsh-autosuggestions $ZSH_CUSTOM/plugins/zsh-autosuggestions

    # zsh-syntax-highlighting
    $ git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```
```
    # In ~/.zshrc  
    plugins={
    git
    web-search
    zsh-autosuggestions
    zsh-syntax-highlighting
    zsh-z
    }

    # others 
    $ brew install tldr  
    $ brew install tmux  
    $ brew install neovim  
    $ brew install tree  
    $ brew install bat
```

# Alias
```
    # In ~/.zshrc
    alias nv='nvim'
    alias q='exit'
```

[My zshrc](https://github.com/kkai0828/Terminal-Settings/blob/main/.zshrc)

# Nvim Settings
[check here](https://github.com/kkai0828/.dotfiles)

