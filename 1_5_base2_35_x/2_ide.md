nano
gedit
vi

apt install vim


VIM

i // insert mode
esc // command mode

i // insert at cursor location
a // append after cursor location
o // insert at a new line
y // copy line
5y / copy 5 lines

dd // delete line
5dd / delete 5 lines

dw // delete word
dl // delete 1 char
p / paste the deleted text

U / undo
redo / ctrl+R

gg / file start
shift g / file end

:5 move to line 5

:wq / save and exit
:qa! / exit

:!ls

!ls - local privileged 

add syntax highlight to vim:
cd ¬
rm .vimrc
touch .vimrc

syntax on
colorscheme delek

vi a.py

#!/usr/bin/python
print('hello world')

chmod +x a.py
./a.py


https://platform.itsafe.co.il/course#day3
סרטון 39
6.41