vim-python-ide
==============

Personal Vim configuration files for developing Python projects on OS X

## How to install

Clone the repo to your local disk first:

```bash
git clone https://github.com/messense/vim-python-ide.git ~/.vim-python-ide
cd ~/.vim-python-ide
git submodule update --init --recursive
# build vimproc
cd .vim/bundle/vimproc.vim && make
# install YouCompleteMe
cd .vim/bundle/YouCompleteMe
./install.sh
```

Softlink `.vim` and `.vimrc` to your HOME directory:

```bash
ln -s ~/.vim-python-ide/.vim ~/.vim
ln -s ~/.vim-python-ide/.vimrc ~/.vimrc
```

You may need to install some Python package to make all this work:

    [sudo] pip install -U jedi flake8 pyflakes

Bonus - screenrc

There is also a screen configuration file `.screenrc` in this project. Using it by:

```bash
ln -s ~/.vim-python-ide/.screenrc ~/.screenrc
```

Key mappings:

* shortcut prefix: C-\
* F2 new screen
* F3 previous screen
* F4 next screen
* F6 detach screen
* F8 rename screen
