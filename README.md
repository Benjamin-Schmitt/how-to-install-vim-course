# how-to-install-vim-course
This short tutorial is aimed and people who are new to both linux and VIM who want VIM to be run in Python3.


Setting up VIM on a new Linux Distro:
1) locate your vimrc file
- go to VIM and do :version. VIM will display the enabled features and the sequence in which VIM will check your several vimrc files. VIM starts by checking the first vimrc file it expects and if none of them are there, it will default to the default vimrc file. 

Note: Most of these files, VIM checks do not exist before you create them. VIM simply expects them because it is common practice to create them.

Note: You don’t want to change the default setting file. 
https://stackoverflow.com/questions/10921441/where-is-my-vimrc-file 


2) Creating a new vimrc
To modify your vimrc file, first you need to create it. 
To create your vimrc, start VIM and do the following:
:e $HOME/.vimrc
This will create a file named .vimrc in your Home directory. This is the file you’re gonna want to modify your VIM with.


3) Guides for editing the vimrc
https://github.com/amix/vimrc
https://realpython.com/vim-and-python-a-match-made-in-heaven/#lets-make-an-ide
https://www.youtube.com/watch?v=vlb3qUiS2ZY&t=342s
https://vimawesome.com/plugin/ncm2
https://www.linode.com/docs/guides/introduction-to-vim-customization/
https://www.youtube.com/watch?v=f7vJzFgUorc&list=PL5iPQU5J96SL9ZY1C_PIbi7iH7qQWNsvf&index=4
https://dev.to/bezirganyan/editor-wars-vim-as-a-perfect-python-ide-19ne
https://medium.com/swlh/setting-up-vim-940eaf179fc8


4) Install Vundle (Packetmanager like PIP)
git clone https://github.com/gmarik/Vundle.vim.git ~/.vim/bundle/Vundle.vim
touch ~/.vimrc


5) How do you know if Vim is compiled with Python3 Support?
Go to VIM and type in:
:versions

No look if the Python and Python3 feature are [+] or [-] 

You can also type (into bash):
python -c "import sys; print(sys.version)"

or open VIM and type:
:python3 import sys; print(sys.version)		#for Python3
:python						#for Python2

https://vi.stackexchange.com/questions/22938/the-python-command-doesnt-work-e319-sorry-the-command-is-not-available-in 

If VIM is compiled in Python2, you may wanna compile it in Python3. 
If the VIM feature is turned of, you may wann do the same.
https://www.reddit.com/r/vim/comments/7fyvgz/easiest_way_to_have_vim_with_python3_support_from/
Solution 1: https://github.com/Shougo/deoplete.nvim#requirements
Solution 2 (works): https://blog.siddharthkannan.in/vim/2019/08/31/compiling-vim-with-python/

