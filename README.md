
# jump (1.0.0)

## Purpose

Opens a file jumping right to a specific line. jump works as wrapper for various text editors and unifies the command to open a text file at a specific line.

## SYNOPSIS 
`jump <editor> +<line_number> <file>`

The option for the line number can also be given as first or last parameter:

`jump +<line_number> <editor> <file>`

`jump <editor> <file> +<line_number>`

## Currently supported editors
- vi, vim
- nano
- leafpad
- pluma
- sublime
- jupp, joe
- kate
- scite
- mcedit
- vis
- ne

### Aliases and symblolic links

Sublime editor exists as sublime-text, but if you have defined an alias or a symbolic link to sublime-text as "sublime", the script will recognize it as the call for the Sublime editor.

Also you can call vim as vi or vim. 

