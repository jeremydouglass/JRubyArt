---
layout: post
title:  "Atom"
permalink: /atom
keywords: ide, ruby, jruby_art, atom
---
### Install Atom ###

See [website][atom] (or scroll to bottom of [releases page for downloads][releases] on github)

For linux ignore any distro version and download latest version (at least 1.10.2) and:-

```bash
sudo dpkg --install atom-amd64.deb # debian, mint, ubuntu
sudo pacman -S atom # Archlinux currently installs 1.10.2
```

Mac/Windows users could just download direct (or homebrew on Mac)

Tough luck if you want the 32 bit version on debian linux

### Install Packages ###

From the atom editor install the `atom-k9` package by [Martin Prout (monkstone)][atom-k9]

While you are at install the `language-jruby-art` package [also by Martin Prout][language] for code snippets (includes a `bare` JRubyArt sketch)

### Watching Sketches (a pseudo REPL)###

_Important_

To watch sketches you should create a new folder (_to avoid watching too many files_) and to reliably pick up the local environment (_eg path to `k9`_) you should start atom from a terminal (_gnome-terminal linux, mintty cygwin_).

```bash
mkdir watch # create a new folder
cd watch # navigate to folder
touch my_sketch.rb # create an empty file
atom my_sketch.rb # fire up atom from command line (to pick up local environment)
```

Make sure you are in `JRuby Art` edit mode (_click on bottom right hand corner to choose_), the use `bare` snippet to create sketch

![enter 'bare'](https://cloud.githubusercontent.com/assets/86850/18698393/e2f48376-7fc1-11e6-80a5-fa8e954bad03.gif)

To avoid need to start from a terminal create a symbolic link to a regular system path to `k9` (eg /usr/local/bin/k9) this easily done/managed on debian linux.

 For a pseudo `REPL` select watch from menu or `ctrl+shift+alt+w`. Then the sketch will reload on `save` after edit.

### To run a sketch ###

To run a sketch, navigate to the sketch (file) and use either menu, or `ctrl+alt+b`.

### What's it look like ###

![atom-k9]({{ site.github.url }}/assets/jwishy.png)

### Expanding / Modifying snippets ###

Navigate to ~/.atom/packages/language-jruby-art/snippets and edit `language-jruby-art.cson`

[language]:https://atom.io/packages/language-jruby-art
[atom-k9]:https://atom.io/packages/atom-k9
[atom]:https://atom.io/
[releases]:https://github.com/atom/atom/releases/tag/v1.10.2