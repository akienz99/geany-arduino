# Geany Syntax highlighting and custom filetype for Arduino files
This repository contains files which enable you to use Geany for creating your Arduino sketches.

What is included:

* File type and extension definition
* Snippets for faster typing of common functions/structures
* Ctags of the standard Arduino librarys to enable code completion

# Installation
* Copy `filetypes.Arduino.conf` to your filedefs in `.config/geany/filedefs/`
* Add the entries in `filetype_extensions.conf` to the corresponding sections in `.config/geany/filetype_extensions.conf`
* Snippets: Add the content of `snippets.conf` to your snippets file in `.config/geany/snippets.conf`
* Ctags: Copy `std.ino.tags` to `.config/geany/tags/`