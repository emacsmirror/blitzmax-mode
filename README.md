# blitzmax-mode - BlitzMax Mode for GNU Emacs

This project adds a new major mode to GNU Emacs for editing BlitzMax source
files. It supports keyword highlighting and automatic indentation.


## Installation

To manually install this extension:

  1. Download the source code and put it somewhere Emacs can find it (probably
     `~/.emacs.d/`).
  2. Add that directory to your `load-path` if it's not yet there: 
    `(add-to-list 'load-path "/path/to/blitzmax-mode")`
  3. Require the mode:
     `(require 'blitzmax-mode)`

Once everything is loaded, blitzmax-mode can be enabled for a buffer by running
`M-x blitzmax-mode`. The mode also associates itself with `.bmx` files, so they
will automatically switch to `blitzmax-mode** when enabled.


## Configuration

**blitzmax-mode** provides the following configuration options:

* `blitzmax-mode-indent` - The number of spaces to indent by. By default
  **blitzmax-mode** indents by 4 spaces which is converted to a single tab.

* `blitzmax-mode-fontify-p` - Disable syntax highlighting by setting this to
  `nil`. `t` by default.

* `blitzmax-mode-capitalize-keywords-p` - Disable automatic capitalization of
  keywords by setting this to `nil`. `t` by default.

* `blitzmax-mode-smart-indent-p` - Disable smart indentation by setting this to
  `nil`. `t` by default.

* `blitzmax-mode-compiler-pathname` - Full pathname to the BlitzMax compiler
  `bmk`. Empty by default.


## Current Features

* Basic syntax highlighting
* Automatic indentation
* Capitalizes keywords automatically


## Planned Features

* Compile current buffer
* Auto-completion
* Integration with bmk
* Integration with blam


## Licence

This file is free software; you can redistribute it and/or modify it under the
terms of the GNU General Public License as published by the Free Software
Foundation; either version 2, or (at your option) any later version.

This file is distributed in the hope that it will be useful, but WITHOUT ANY
WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with GNU
Emacs; see the file COPYING.  If not, write to the Free Software Foundation,
Inc., 59 Temple Place - Suite 330, Boston, MA 02111-1307, USA.