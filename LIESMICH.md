
# jump (1.2.0)

## Leistung

Öffnet eine Textdatei und springt direkt zu eine bestimmten Zeile. jump ist ein Wrapper-Programm, das den dafür notwendigen Aufruf für diverse Texteditoren und Text-Viewer vereinheitlicht.

## Aufrufsyntax
`jump <editor> +<line_number> <file>`

Die Option mit der Zeilennummer kann ebenso gut als erster oder letzter Prameter angegeben werden:

`jump +<line_number> <editor> <file>`

`jump <editor> <file> +<line_number>`

### Beispielaufruf

`jump leafpad +220 meinscript.sh`

## Unterstützte Texteditoren und Text-Viewer
- vi, vim
- nano
- leafpad
- pluma
- sublime-text 
- jupp, joe, jstar, jpico, jmacs
- kate
- scite
- mcedit
- cream
- vis
- ne
- xed
- less
- more
- most

### Aliase

sublime-text kann als sublime aufgerufen werden, wenn im System ein Alias oder ein symbolischer Link angelegt wurde, der auf sublime-text verweist. 

