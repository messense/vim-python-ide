vim-python-ide
==============

Personal Vim configuration files for developing Python projects on OS X

## How to install

Clone the repo to your local disk first:

    git clone https://github.com/messense/vim-python-ide.git ~/vim
    cd ~/vim
    git submodule init && git submodule update

Copy `.vim` and `.vimrc` to your HOME directory:

    cp ~/vim/.vim ~/.vim
    cp ~/vim/.vimrc ~/.vimrc

You may need to install a Python package `jedi` to make all this work:

    [sudo] pip install jedi
