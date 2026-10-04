# bindkey

> Add hotkeys to Z shell.
> See also: `zle`.
> More information: <https://zsh.sourceforge.io/Doc/Release/Zsh-Line-Editor.html#Zle-Builtins>.

- List all existing hotkeys:

`bindkey`

- Bind a hotkey to a specific command:

`bindkey "{{^k}}" {{kill-line}}`

- Bind a hotkey to a specific key sequence:

`bindkey -s '^o' 'cd ..\n'`

- list keymaps:

`bindkey -l`

- List all hotkeys in a keyMap:

`bindkey -M {{main}}`

- Enable vi mode:

`bindkey -v`

- Enable emacs mode (default mode):

`bindkey -e`

- Check which mode is active (vi or emacs):

`bindkey -lL main | grep -Eo 'viins|emacs'`
