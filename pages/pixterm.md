# pixterm

> Image printing in the terminal.
> See also: `chafa`, `catimg`.
> More information: <https://github.com/eliukblau/pixterm#cool-screenshots>.

- Render a static image directly in the terminal:

`pixterm {{path/to/file}}`

- Use the image's original aspect ratio:

`pixterm -s 2 {{path/to/file}}`

- Specify a custom aspect ratio using a specific number of terminal rows and columns:

`pixterm -tr {{24}} -tc {{80}} {{path/to/file}}`

- Filter the output with a matte background color and character dithering:

`pixterm -m {{000000}} -d 2 {{path/to/file}}`
