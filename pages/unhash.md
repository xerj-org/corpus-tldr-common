# unhash

> Remove hashed executable locations.
> See also: `hash`.
> More information: <https://zsh.sourceforge.io/Doc/Release/Shell-Builtin-Commands.html>.

- Remove a specific command from the hash table:

`unhash {{command}}`

- Unhash non-suffix aliases:

`unhash -a {{alias}}`

- Unhash suffix aliases:

`unhash -s {{alias}}`

- Unhash shell functions:

`unhash -f {{function}}`

- Unhash directories:

`unhash -d {{directory}}`

- Unhash every function that matches a pattern:

`unhash -f -m "{{pattern}}"`
