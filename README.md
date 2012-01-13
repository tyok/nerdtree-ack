# NERDtree + Ack.vim

This plugin add capability to search in folders via NERDtree. The search use ack.vim from the master branch (<http://github.com/mileszs/ack.vim/tree/master>).
This is ripped off from [NERDTree & ack plugin](http://www.vim.org/scripts/script.php?script_id=3357) by Tudor Barbu. It just doesn't fit my taste, so, yeah.

## How to Install

1. Install ack.vim first from <http://github.com/mileszs/ack.vim/tree/master>. Or you can use [my branch](https://github.com/tyok/ack.vim) whose behavior is IMHO more NERDtree-friendly.
1. Copy the plugin file to your `.vim/plugin` directory, or install via pathogen/vundle

## How to Use

1. Open NERDtree
1. Point to a directory
1. Press `ms`
1. Enter search term (e.g. `control\ panel -i`)
1. Profit!

## Features

1. Doesn't change current open buffers! This feature is what necessitate the use of latest ack.vim
1. Uses ack.vim syntax:
    1. Use `\ ` to write a space (e.g. `control\ panel`)
    1. Or enclose the term in quotes (e.g. `"control panel"`)
    1. The default behavior is case sensitive. Use `-i` params for case insensitive (e.g. `"control panel" -i`)
1. Uses ack.vim buffer behavior
