
# jump (1.2.3)

## Leistung

Öffnet eine Textdatei und springt direkt zu eine bestimmten Zeile. jump ist ein Wrapper-Programm, das den dafür notwendigen Aufruf für diverse Texteditoren und Text-Viewer vereinheitlicht.

## Aufrufsyntax
`jump <editor> +<line_number> <file>`

`jump --hilf`

`jump --supported`

`jump --aliase`

`jump --version`

Die Option mit der Zeilennummer kann ebenso gut als erster oder letzter Prameter angegeben werden:

`jump +<line_number> <editor> <file>`

`jump <editor> <file> +<line_number>`

### Optionen

| Option        | Wirkung                                                      |
| ------------- | ------------------------------------------------------------ |
| `--hilf`      | Aufruf der Hilfeseite                                        |
| `--supported` | Listet die unterstützten Programme auf                       |
| `--aliase`    | Listet die aktuellen Programmaliase auf.                     |
| `--version`   | Zeigt die Programmversion an.                                |
| `-#`          | Gibt nur die Versionsnummer des Programms aus, zum Beispiel "1.2.0". |

### Beispielaufruf

`jump leafpad +220 meinscript.sh`

## Unterstützte Texteditoren und Text-Viewer
> cream, emacs, geany, gedit, gvim, jed, jmacs, joe, jpico
jstar, jupp, kak (kakoune), kate, kwrite, leafpad, less
less, mcedit, medit, more, most, nano, ne, nvim, pico, pluma,
scite, sublime, vim, vis, xed

### Programminterne Aliase

Unabhängig von den Aliasdefinitionen des Linux-Systems erkennt das Programm eine Reihe Aliase, Kürzel, die es intern in einen gültigen Programmnamen übersetzt. Diese Aliase sind in einer gesonderten Datei namens `.jump_aliases` definiert, die Home-Verzeichnis des aktuellen Anwenders gesucht wird. Darin kann man Aliase nach seinem eigenen Geschmack definieren. Die aktuell gültigen Aliase werden angezeigt, wenn man das Kommando `jump -aliases` gibt.   

sublime_text kann auch als sublime aufgerufen werden, wenn nur im System ein Alias oder ein symbolischer Link angelegt wurde, der auf sublime_text verweist. 

