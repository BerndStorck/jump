
# jump (1.2.0)

## Purpose

Opens a file jumping right to a specific line. jump works as wrapper for various text editors and unifies the command to open a text file at a specific line.

## SYNOPSIS 
`jump <editor> +<line_number> <file>`

`jump --help|-h`

`jump --supported`

`jump --aliases`

`jump --version`

The option for the line number can also be given as first or last parameter:

`jump +<line_number> <editor> <file>`

`jump <editor> <file> +<line_number>`

### Optionen

| Option           | Effect                                     |
| ---------------- | ------------------------------------------ |
| `--help` or `-h` | Shows the help page.                       |
| `--supported`    | Lists the supported programs.              |
| `--aliases`      | Lists the current program aliases.         |
| `--version`      | Displays the program version.              |
| `-#`             | Displays the version number. e. g. "1.2.0" |

## Currently supported editors and viewers

> cream, emacs, geany, gedit, gvim, jed, jmacs, joe, jpico
jstar, jupp, kak (kakoune), kate, kwrite, leafpad, less
less, mcedit, medit, more, most, nano, ne, nvim, pico, pluma,
scite, sublime, vim, vis, xed

### Aliases and symbolic links

Independent of the alias definitions of the Linux system, the program recognizes a number of aliases, of abbreviations, which it translates internally into a valid program name. These aliases are defined in a separate file called `.jump_aliases`, which searches the home directory of the current user. In this file you can define aliases according to your own taste. The currently valid aliases are displayed when you give the command `jump --aliases`. 

Sublime editor exists as sublime-text, but if you have defined an alias or a symbolic link to sublime-text as "sublime", the script will recognize it as the call for the Sublime editor, even if you have not defined a jump-internal alias for it. Also you can call vim as vi or vim. 

