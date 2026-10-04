# boxes

> Draw, remove, and repair ASCII art boxes.
> More information: <https://boxes.thomasjensen.com/boxes-man-1.html>.

- Draw a box around a string:

`echo "{{string}}" | boxes`

- Remove a box from a string:

`echo "{{string}}" | boxes {{[-r|--remove]}}`

- Specify the box design:

`echo "{{string}}" | boxes {{[-d|--design]}} {{parchment}}`

- Specify the box size (in columns by lines):

`echo "{{string}}" | boxes {{[-s|--size]}} {{10}}x{{5}}`

- Align the box text horizontally (at left, center, or right):

`echo "{{string}}" | boxes {{[-a|--align]}} h{{l|c|r}}`

- Align the box text vertically (at top, center, or bottom):

`echo "{{string}}" | boxes {{[-a|--align]}} v{{t|c|b}}`

- justify the box text (at left, center, or right):

`echo "{{string}}" | boxes {{[-a|--align]}} j{{l|c|r}}{{vt}}`
