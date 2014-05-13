Vim Syntax for Pebble Smartwatch API
------------------------------------
This is a [Vim](http://vim.org) syntax file for the
[Pebble Smartwatch](http://getpebble.com) SDK 2.0 API.

This adds syntax keywords for all the Pebble types, constants, and functions.

Installing
----------
If you're using [Pathogen](https://github.com/tpope/vim-pathogen), clone this
repository into `~/.vim/bundle/pebble-syntax` to install.

If not, just drop `syntax/pebble.vim` into your `~/.vim/syntax/` directory.

Getting This to Work
--------------------
Because Pebble uses regular `*.c` and `*.h` files, you will have to tell Vim
to load `pebble.vim` instead of the standard `c.vim`. I did this by putting
all my Pebble projects in the same parent directory and added this `autocmd`
to my `~/.vimrc`:

    autocmd BufNewFile,BufRead ~/pebble-dev/*.{c,h} set syntax=pebble

Alter the path to taste, of course.

You can also use a [modeline](http://vim.wikia.com/wiki/Modeline_magic) like
`/* vim: set syntax=pebble: */` if you're into that.
