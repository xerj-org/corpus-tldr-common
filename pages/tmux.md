# tmux

> Terminal multiplexer.
> It allows multiple sessions with windows, panes, and more.
> See also: `zellij`, `screen`, `herdr`.
> More information: <https://github.com/tmux/tmux>.

- Start a new session:

`tmux`

- Start a new named session:

`tmux {{[new|new-session]}} -s {{name}}`

- List existing sessions:

`tmux {{[ls|list-sessions]}}`

- Attach to a named session (target can be omitted to attach to the most recently used session):

`tmux {{[a|attach]}} -t {{name}}`

- Detach from the current session (inside a tmux session):

`<Ctrl b><d>`

- Create a new window (inside a tmux session):

`<Ctrl b><c>`

- Switch between sessions and windows (inside a tmux session):

`<Ctrl b><w>`

- Kill a session by target name:

`tmux kill-session -t {{name}}`
