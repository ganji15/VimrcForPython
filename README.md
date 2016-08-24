# PythonVimPlugin

## Installation
###1 git clone https://github.com/ganji15/PythonVimPlugin.git
###2 cd PythonVimPlugin, then cp .vim and .vimrc to ~
###3 install [ctags](#ctags) and [jedi](#jedi) and [pylint](#pylint)
* sudo apt-get install ctags 
* pip install jedi
* sudo apt-get install pylint

###4 generate tags
* cd /usr/local/
* sudo ctags -R /usr/local/lib/python2.7/dist-packages/

###5 configure pylint
* sudo touch /etc/pylintrc
* sudo chmod 777 /etc/pylintrc
* pylint --generate-rcfile > /etc/pylintrc
* sudo gedit /etc/pylintrc, find \[MESSAGE CONTROL\] and add "[#disable=line-too-long, missing-docstring, wildcard-import, unused-wildcard-import, bad-whitespace, trailing-whitespace](#pylint-disable)"

###6 go to vim, run ":BundleInstall"
###7 compile YouCompleteMe
* More details:https://github.com/Valloric/YouCompleteMe

## Features
| Plugins        | Features | key trigger  |
|:------------- |:-------------|:------------- |
| powerline     |  fancy status bar |  |
| delemitMate      | barkets pair completition|   |
| nerdtree | files navigation bar      |  press \<F6\> to toggle|
| tagbar   | code function lists | press \<F7\> to toggle |
| ycm    | code completition      |   press \<ctrl-n\> and \<ctrl-p\> to comlete|
| ctags | find defination && delearation      | press \<F8\> to generate tags &&  press \<ctrl-]\> jump && \<ctrl-t\> jump back|
| ctrlp     | find files fast|  press \<ctrl-p\> to trigger |
| nerd commender    | code commenter      |   press \\cc to comment && \\cu to undo comment |
| simpyfold     | code fold|  press \<space\> or za to fold code |
| syntastic    | syntastic check | press \<F10\> to check and \<F9\> to close|
| pydocstring | add doc string | press <ctrl-a> to add doc string|

## Window
![Window](https://github.com/ganji15/VimrcForPyhon/blob/master/python-vim-plugin.png)
