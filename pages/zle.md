# zle

> Manage Zsh Line Editor widgets.
> Note: Some operations require ZLE to be active (typically inside a user-defined widget).
> See also: `bindkey`.
> More information: <https://zsh.sourceforge.io/Doc/Release/Zsh-Line-Editor.html#Zle-Builtins>.

- list user-defined widgets:

`zle -l`

- list all widgets, including built-in ones:

`zle -la`

- Create a New user-defined widget (function defaults to same name as widget):

`zle -N {{widget_name}} {{optional_shell_function_name}}`

- Delete a widget:

`zle -D {{widget_name}}`

- Create an Alias of a widget:

`zle -A {{original_widget}} {{alias_name}}`

- Invoke a widget from inside another widget function (requires active ZLE):

`zle {{widget_name}}`

- Push text into ZLE's input queue as if it were typed (requires active ZLE):

`zle -U "{{text}}"`
