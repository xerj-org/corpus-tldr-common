# chkrootkit

> Scan system for rootkits.
> More information: <https://manned.org/chkrootkit>.

- Enable quiet mode and suppress normal test results:

`chkrootkit -q`

- Enable expert mode and produce additional outputs:

`chkrootkit -x`

- Enable debug mode to show all output:

`chkrootkit -d`

- Specify excluded files for some tests:

`chkrootkit -e "{{path/to/file}}"`

- Specify a directory as the root for testing (e.g. mounted `ext` drives):

`chkrootkit -r {{path/to/directory}}`

- Ignore nfs-mounted directories:

`chkrootkit -n`

- Invoke Tests and ignore specific filesystem types:

`chkrootkit -T {{filesystemtype}}`

- Generate list of available tests:

`chkrootkit -l`
