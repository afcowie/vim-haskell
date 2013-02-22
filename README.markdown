Syntax highlighting for Haskell source files
============================================

1. Parsing
----------

Checkout this repository (you know how to do this part):

    $ cd ~/src
    $ git clone git://github.com/afcowie/vim-haskell.git
    [ ... poke around ...]
    $ cd ~

Then make a symlink from your runtime syntax directory to ensure this file is
loaded.

    $ mkdir ~/.vim/syntax
    $ ln -s ~/src/vim-haskell/syntax/haskell.vim ~/.vim/syntax

You could just copy the file in instead, but version controlling stuff
in places like `.vim` can be tricky.

2. Colouring
------------

And then, you'll want colours. This set is based on the [Tango colour
palette](http://tango.freedesktop.org/Tango_Icon_Theme_Guidelines#Color_Palette)
which is an entirely arbitrary choice, except that as a group they are very consistent
and entirely complementary to each other.

	highlight LineNr guifg=#eeeeec

	highlight Constant ctermfg=Blue guifg=#73d216
	highlight String ctermfg=Blue cterm=bold guifg=#204a87 gui=bold
	highlight Comment ctermfg=Grey guifg=#888a85
	highlight Special guifg=#ad7fa8
	highlight PreProc guifg=#f57900
	highlight Identifier guifg=#729fcf
	highlight Statement guifg=#8f5902
	highlight Type guifg=#73d216 gui=bold
	highlight hsType guifg=black gui=bold
	highlight hsImportLabel guifg=#73d216 gui=bold
	highlight hsImport guifg=black gui=bold
	highlight hsModuleName guifg=black gui=bold
	highlight hsLineComment guifg=#888a85
	highlight hsBlockComment guifg=#c4a000

It's like colouring inside the lines, only for adults!

AfC

