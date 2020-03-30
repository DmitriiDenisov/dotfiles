### `ZSH`:

1. Isntall zsh

2. Install 'Oh my zsh', see 'Basic Installation':
https://github.com/ohmyzsh/ohmyzsh

Themes:
https://github.com/ohmyzsh/ohmyzsh/wiki/Themes

3. Customize vim and zsh:

https://github.com/alex-33/dotfiles

if problems (ADD NAME OF ERROR + SCREEN)

then
Ubuntu => 
```
sudo apt-get install vim-gui-common
sudo apt-get install vim-runtime
```

Mac => `brew install vim`

aliases (add to ~/.zshrc), example:
`alias virtual="ssh mail_2020q1@virtual-client.bigdatateam.ru -L 50070:virtual-master:50070"`


Useful plagins:

1. Auto suggestions, see 'Oh My Zsh':

https://github.com/zsh-users/zsh-autosuggestions

2. Spelling correction:

You enable the feature by adding `setopt correct` to your config `~/.zshrc` and then resourcing your configuration with the command `source ~/.zshrc`


## HotKeys in CLI:
cmd + enter - FullScreen
ctrl+L - clear
ctrl+u - clear typed 
ctrl+k - clear the line after cursor