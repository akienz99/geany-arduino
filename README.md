# Geany Syntax highlighting and custom filetype for Arduino files
This repository contains files which enable you to use Geany for creating your Arduino sketches.

## What is included:

* File type and extension definition
* Snippets for faster typing of common functions/structures
* Ctags of the standard Arduino libraries to enable code completion

## Installation

* Copy `filetypes.Arduino.conf` to your filedefs in `.config/geany/filedefs/`
* Add the entries in `filetype_extensions.conf` to the corresponding sections in `.config/geany/filetype_extensions.conf`
* Snippets: Add the content of `snippets.conf` to your snippets file in `.config/geany/snippets.conf`
* Ctags: Copy `std.ino.tags` to `.config/geany/tags/`

## Building your own tagfile

As you might use a different set of libraries than the standard Arduino libraries,
you might want to build your own tagfile. To do that, create a folder and copy
all of the libraries you want to tag into it. Then copy all of the standard libraries
https://github.com/akienz99/arduino-library-files to that folder.

To create the tags, open a terminal in that folder and run

`arduino-ctags -R .`

and to use them in Geany, rename and move the tags file to your tags folder

`mv tags ~/.config/geany/tags/std.ino.tags`

Now you have updated Ctags for your needs!