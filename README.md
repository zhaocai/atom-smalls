# smalls

Rapid cursor positioning across any visible chars with search and jump.

# Development state.

Alpha.

# Features

* Search and jump to character across visible panes.
* Flashing cursor position on landing(enbaled by default).
* [eazymotion](https://github.com/easymotion/vim-easymotion) style label jump.
* Port of my [vim-smalls](https://github.com/t9md/vim-smalls/blob/master/README.md).

# How to use

1. Start smalls-mode with `smalls:start`
2. Input character then `enter` to the mini-panel.
3. Choose overlaid label then you cursor landed to new position with flashing.

# Commands

* `smalls:start`: Start smalls jumping mode.

# Keymap
No keymap by default.

e.g.

```coffeescript
'atom-text-editor:not([mini])':
  'ctrl-s': 'smalls:start'
```

* My setting, I'm [vim-mode](https://atom.io/packages/vim-mode) user.
NOTE `;` is bound to `vim-mode:repeat-find`, very important command.
So If you follow my keymap, you'd better assign `vim-mode:repeat-find` to other
keybind.

```coffeescript
'atom-text-editor.vim-mode.command-mode':
  ';': 'smalls:start'
```

# Similar packages

Atom
* [jumpy](https://atom.io/packages/jumpy)
* [easy-motion](https://github.com/adrian-budau/easy-motion)
* [quick-jump](https://atom.io/packages/quick-jump)
* [QuickJumpPlus](https://atom.io/packages/QuickJumpPlus)

Vim
* [vim-easymotion](https://github.com/easymotion/vim-easymotion)
* [clever-f](https://github.com/rhysd/clever-f.vim)
* [vim-sneak](https://github.com/justinmk/vim-sneak)
* [vim-seek](https://github.com/goldfeld/vim-seek)
* [vim-smalls](https://github.com/t9md/vim-smalls)

Emacs
* [ace-jump-mode](https://github.com/winterTTr/ace-jump-mode)

IntelliJ
* [AceJump](https://github.com/johnlindquist/AceJump)

# TODO

* [x] Use panel to read input from user
* [ ] Customizble style
* [ ] Unlock scroll cursor?
* [ ] Narrowing based on grammar scope?
