# oh-my-zsh-powerlevel9k-theme
Most awesome terminal shell you have ever seen!

## Linux CentOS 7
testing on fresh new `robot` user:

```bash
sudo yum install -y git curl zsh vim
sudo adduser -G wheel -s /bin/zsh -m robot
sudo su -- robot

cd
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
git clone https://github.com/bhilburn/powerlevel9k.git ~/.oh-my-zsh/custom/themes/powerlevel9k
vi ~/.zshrc

#ZSH_THEME="robbyrussell"
ZSH_THEME="powerlevel9k/powerlevel9k"
POWERLEVEL9K_MODE="nerdfont-complete"
POWERLEVEL9K_VCS_SHORTEN_LENGTH=4
POWERLEVEL9K_VCS_SHORTEN_MIN_LENGTH=11
POWERLEVEL9K_VCS_SHORTEN_DELIMITER=".."
POWERLEVEL9K_LEFT_PROMPT_ELEMENTS=(os_icon dir vcs status)
POWERLEVEL9K_RIGHT_PROMPT_ELEMENTS=(root_indicator time)
POWERLEVEL9K_TIME_FORMAT='%D{%S:%M:%H}'
POWERLEVEL9K_PROMPT_ON_NEWLINE=false
```

finally install [Hack Nerd Regular Font](https://github.com/ryanoasis/nerd-fonts/raw/master/patched-fonts/Hack/Regular/complete/Hack%20Regular%20Nerd%20Font%20Complete.ttf) in your system to see all awesomness!

An we are done!
