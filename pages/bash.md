# bash

> Bourne-Again SHell, an `sh`-compatible command-line interpreter.
> See also: `zsh`, `!`.
> More information: <https://www.gnu.org/software/bash/manual/bash.html#Invoking-Bash>.

- Start an interactive shell session:

`bash`

- Start an interactive shell session without loading startup configs:

`bash --norc`

- Execute specific commands:

`bash -c "{{echo 'bash is executed'}}"`

- Execute a specific script:

`bash {{path/to/script.sh}}`

- Execute a specific script, printing each command before executing it:

`bash -x {{path/to/script.sh}}`

- Execute a specific script and stop at the first error:

`bash -e {{path/to/script.sh}}`

- Execute specific commands from `stdin`:

`{{echo "echo 'bash is executed'"}} | bash`

- Start a restricted shell session:

`bash {{[-r|--restricted]}}`
