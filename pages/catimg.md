# catimg

> Image printing in the terminal.
> See also: `pixterm`, `chafa`.
> More information: <https://manned.org/catimg>.

- Print a JPEG, PNG, or GIF to the terminal:

`catimg {{path/to/file}}`

- Double the resolution of an image:

`catimg -r 2 {{path/to/file}}`

- Disable 24-bit color for better terminal support:

`catimg -t {{path/to/file}}`

- Specify a custom width or Height:

`catimg {{-w|-H}} {{40}} {{path/to/file}}`
