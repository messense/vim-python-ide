vim-python-ide
==============

Personal Vim configuration files for developing Python projects on OS X

## How to install

Clone the repo to your local disk first:

```bash
git clone https://github.com/messense/vim-python-ide.git ~/.vim-python-ide
cd ~/.vim-python-ide
git submodule init && git submodule update
# build vimproc
cd .vim/bundle/vimproc.vim && make
# get jedi
cd .vim/bundle/jedi-vim && git submodule update --init
# install YouCompleteMe
cd .vim/bundle/YouCompleteMe
git submodule update --init --recursive
./install.sh
```

Softlink `.vim` and `.vimrc` to your HOME directory:

```bash
ln -s ~/.vim-python-ide/.vim ~/.vim
ln -s ~/.vim-python-ide/.vimrc ~/.vimrc
```

You may need to install some Python package to make all this work:

    [sudo] pip install -U jedi flake8 pyflakes
