# gofumpt

> Strictly format Go files.
> See also: `gofmt`.
> More information: <https://github.com/mvdan/gofumpt#gofumpt>.

- Format Go files:

`gofumpt -w {{path/to/directory}}`

- list files whose formatting differs from `gofumpt`:

`gofumpt -l {{path/to/directory}}`

- Report all errors:

`gofumpt -e {{path/to/directory}}`

- Display diffs:

`gofumpt -d {{path/to/directory}}`

- Format Go files with stricter rules:

`gofumpt -extra {{path/to/directory}}`

- Display diffs with stricter rules:

`gofumpt -extra -d {{path/to/directory}}`

- Display help:

`gofumpt {{[-h|--help]}}`
