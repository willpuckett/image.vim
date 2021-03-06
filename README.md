# image.vim, with Python3

Forked from ashisha/image.vim as the PR to update to Python3 went unanswered for years.


View images in Vim, because Vim is awesome!

![](https://github.com/ashisha/image.vim/blob/master/screenshot/image.vim.jpg)

When I work in ssh it's great to view images with:

```vim 
:autocmd BufEnter *.png,*.jpg,*gif exec "! ~/.iterm2/imgcat ".expand("%") | :bw
```

but imgcat doesn't work with mosh :(

image.vim does :)


Features
=========
* Let's you open (preview) images in Vim!
* It's safe, never modifies the original image (unless you force write)


Requirements
============
Python3 

* Vim with *python* support. You can verify if your Vim is compiled with python using:
  
  `vim --version | grep python`
  
  Python 2 reached EOL Jan 1, 2020.

  If you see `+python3`, your Vim has python3 support. If not, figure out how to get one.

* Also needs the Python library PIL. You can install PIL using `pip3 install Pillow`

Installation
============
* [Pathogen](https://github.com/tpope/vim-pathogen)
  *  `git clone https://github.com/willpuckett/image.vim ~/.vim/bundle/image.vim`
* [Vundle](https://github.com/gmarik/vundle)
  * `Plugin 'willpuckett/image.vim'`
* [NeoBundle](https://github.com/Shougo/neobundle.vim)
  * `NeoBundle 'willpuckett/image.vim'`
* Manual
  * Copy image.vim into your `~/.vim/plugin/` directory

Cheers!
