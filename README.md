vim-python-ide
==============

Personal Vim configuration files for developing Python projects on OS X

## How to install

Clone the repo to your local disk first:

```bash
git clone https://github.com/messense/vim-python-ide.git ~/vim
cd ~/vim
git submodule init && git submodule update
# build vimproc
cd .vim/bundle/vimproc.vim && make
```

Copy `.vim` and `.vimrc` to your HOME directory:

```bash
cp ~/vim/.vim ~/.vim
cp ~/vim/.vimrc ~/.vimrc
```

You may need to install some Python package to make all this work:

    [sudo] pip install -U jedi flake8
