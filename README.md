# vimrc for Debian 9 v1.0
# rampage nps
# my best vimrc configuration

# Install requirement for Vim 
  apt -y install ncurses-dev libncurses5-dev libncursesw5-dev vim-gtk vim-gnome vim-athena


# Download it
git clone https://github.com/vim/vim.git

# You need to uninstall your actual vim and compile it again
 ./configure –enable-multibyte \
 --enable-fontset             
 --enable-xim 
 --enable-gui=no 
 --enable-pythoninterp=yes
 --enable-rubyinterp=dynamic
 --enable-perlinterp
 --enable-cscope
 --enable-sniff
 --with-x
 --with-compiledby=erocpil
 --with-features=huge
 --with-python-config-dir=/usr/lib/python2.7/config-x86_64-linux-gnu
 --enable-luainterp 
# Compile and install
make && make install

