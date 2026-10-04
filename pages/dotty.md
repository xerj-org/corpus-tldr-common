# dotty

> A customizable interactive graph editor for the X Window System.
> Note: This command is deprecated.
> More information: <https://graphviz.org/pdf/dotty.1.pdf>.

- Open a graph file (`.gv` or `.dot`) in the Dotty editor:

`dotty {{path/to/graph.gv}}`

- Start Dotty with the Version information displayed:

`dotty -V`

- Set the layout mode to synchronous or asynchronous:

`dotty -lm {{sync|async}} {{path/to/graph.gv}}`

- Set the message verbosity level (`0` for minimal, `1` for detailed):

`dotty -el {{0|1}} {{path/to/graph.gv}}`
