# yj

> Convert between YAML, TOML, JSON, and HCL, preserving map order.
> More information: <https://github.com/sclevine/yj>.

- Convert yAML to JSON (default) from `stdin` and write the result to `stdout`:

`yj < {{file.yml}} -y`

- Convert tOML to yAML:

`yj < {{file.toml}} -ty`

- Convert jSON to tOML with indentation:

`yj < {{file.json}} -jti`

- Convert HcL to jSON:

`yj < {{file.hcl}} -cj`

- Convert yAML to HcL ignoring inf/naN conversion:

`yj < {{file.yml}} -ycn`

- Display version:

`yj -v`
