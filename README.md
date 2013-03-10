# Brackets Vim Mode
An extension meant to bring vim-like functionality to Adobe's 
[Brackets](http://brackets.io).

Pretty much all of the Vim keymapping is from 
[CodeMirror](http://codemirror.net)'s /keymap/vim.js, but I modified
things very heavy-handedly. The two files will probably need to 
be maintained in parallel until I can figure out a way to do this
natively in Brackets.

## Installing Vimderbar
0. Copy this repository into your brackets extensions folder.
0. Run Brackets. 
0. Toggle Vimderbar via Brackets' menu with "View > Enable Vimderbar".
  * Modify settings.js to choose whether or not this should be enabled by default.

## Features
+ Basic vim keybindings (hjkl, yy, dd, p, P, o, O, gg, G, etc.).
+ Search function (`/`).
+ Modes: Normal, Insert, Visual (Visual-line, too).

## Limitations
+ `:` commands are sloppy, only one can be performed at a single time.
+ Can't yet perform complex `:` commands (like `:1,8d`)
+ Reverse search (`?`) has been disabled to accommodate the native 
search.
+ Visual mode selection is kind of broken (visual line mode 
seems to work fine).
+ Can't yet yank or delete selected text using `yy` or `dd`. 
Please use `cmd-c`/`ctrl-c` and `cmd-v`/`ctrl-v` instead.
+ Saving with `:w` can cause the cursor to jump to a higher part of the 
file (inconsistently observed).
+ Funky indentation (tabs instead of spaces? not sure). 
+ `:` does not yet have "history" (e.g. pressing Up to get previous commands).

## Contributing
Please do, by all means, hack on this extension. For coding conventions, review the 
[Brackets Coding Conventions]
(https://github.com/adobe/brackets/wiki/Brackets%20Coding%20Conventions).

Thanks!

## Licence
I'd say WTFPL, but the MIT disclaimers are important(see main.js).