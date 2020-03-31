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

3. zsh-syntax-highlighting, see installation 'Oh-my-zsh':

https://github.com/zsh-users/zsh-syntax-highlighting/blob/master/INSTALL.md

4. Enable mouse in vim:

https://www.youtube.com/watch?v=kvmD_N1iIwg

5. Add shortcut for cut and paste:

https://www.youtube.com/watch?v=E_rbfQqrm7g&t=239s

6. Ranger:

brew install ranger

To draw borders:
1)ranger --copy-config=all
2) path to config: ~/.config/rc.conf
3) Inside config file: set draw_borders true

To enable preview of images:
1) set preview_images true
2) set preview_images_method iterm2

7. Midnight commander (mc):

brew install midnight-commander

if backspace in insert mode does not work:
add `set backspace=indent,eol,start` to `.vimrc` file


8. Auto-Complete in vim:

- add `Plugin 'Valloric/YouCompleteMe'` in .vimrc file
- run in vim :PluginInstall
- cd ~/.vim/bundle/YouCompleteMe/
- ./install.py
- ./install.py --clang-completer
If it's not working again run :PluginInstall

Source: https://programmer.group/installation-of-vim-plug-in-youcompleteme-for-mac.html

9. Syntastic

Install:
add to .vimrc plugin
Plugin 'vim-syntastic/syntastic'
Plugin 'nvie/vim-flake8'

Settings:
set statusline+=%#warningmsg#
set statusline+=%{SyntasticStatuslineFlag()}
set statusline+=%*

let g:syntastic_always_populate_loc_list = 1
let g:syntastic_auto_loc_list = 1
let g:syntastic_check_on_open = 1
let g:syntastic_check_on_wq = 0

For using python3 checker instead of python2
let g:syntastic_python_python_exec = 'python3'
let g:syntastic_python_checkers = ['python']

Source:
https://github.com/vim-syntastic/syntastic

10. NERDTree 

Install: 

Plugin 'scrooloose/nerdtree'
Plugin 'jistr/vim-nerdtree-tabs'

Create file/rename file/remove file:
https://sookocheff.com/post/vim/creating-a-new-file-or-directoryin-vim-using-nerdtree/

Switch between windows:
https://superuser.com/questions/280500/how-does-one-switch-between-windows-on-vim

<C-w>n - :new horizontal split (editing a new empty buffer)
<C-w>s - :split window horizontally (editing current buffer)
<C-w>v - :vsplit window vertically (editing current buffer)
<C-w>c - :close window
<C-w>o - close all windows, leaving :only the current window open

Source:
https://github.com/preservim/nerdtree

## HotKeys in CLI:
cmd + enter - FullScreen
ctrl+L - clear
ctrl+u - clear typed 
ctrl+k - clear the line after cursor

## HotKeys in vim:
u - undo
ctrl+r - redo
Ctrl-o, 0 beginning of line
Ctrl-o, $ end of line
Ctrl-o, f, y find first y in sentence

Shft+0 - start of next line (NOT i mode)
shift+$ - beggining of line (NOT i mode)





for ctrl+A for select all:

map <C-a> <esc>ggVG<CR>
