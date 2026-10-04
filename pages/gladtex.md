# gladtex

> A LaTeX formula preprocessor for HTML files.
> It converts LaTeX formulas to images.
> More information: <https://manned.org/gladtex>.

- Convert to HTML:

`gladtex {{path/to/input.htex}}`

- Save the converted file to a specific output file:

`gladtex {{path/to/input.htex}} -o {{path/to/output.html}}`

- Save the generated images to a specific directory:

`gladtex {{path/to/input.htex}} -d {{path/to/image_output_directory}}`

- Set image resolution (in dpi, default is 100):

`gladtex {{path/to/input.htex}} -r {{resolution}}`

- keep LaTeX files after conversion:

`gladtex {{path/to/input.htex}} -k`

- Set background and foreground color of the images:

`gladtex {{path/to/input.htex}} -b {{background_color}} -f {{foreground_color}}`

- Convert Markdown to HTML using `pandoc` and `gladtex`:

`pandoc {{[-s|--standalone]}} {{[-t|--to]}} html --gladtex {{path/to/input.md}} | gladtex -o {{path/to/output.html}}`
