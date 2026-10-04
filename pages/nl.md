# nl

> Number lines from a file or from `stdin`.
> More information: <https://manned.org/nl.1p>.

- Number non-blank lines in a file:

`nl {{path/to/file}}`

- Read from `stdin`:

`{{command}} | nl -`

- Number all body lines including blank lines or do not number body lines:

`nl -b {{a|n}} {{path/to/file}}`

- Number only the body lines that match a basic `regex` (BRE) pattern:

`nl -b p'FooBar[0-9]' {{path/to/file}}`

- Use a specific increment for line numbering:

`nl -i {{increment}} {{path/to/file}}`

- Specify the line numbering format to right or left justified, keeping leading zeros or not:

`nl -n {{rz|ln|rn}}`

- Specify the line numbering's width (6 by default):

`nl -w {{col_width}} {{path/to/file}}`

- Use a specific string to separate the line numbers from the lines (`TAB` by default):

`nl -s {{separator}} {{path/to/file}}`
