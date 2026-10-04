# tar

> Archiving utility.
> Often combined with a compression method, such as `gzip` or `bzip2`.
> More information: <https://www.gnu.org/software/tar/manual/tar.html>.

- create an archive and write it to a file:

`tar cf {{path/to/target.tar}} {{path/to/file1 path/to/file2 ...}}`

- create a gzipped archive and write it to a file:

`tar czf {{path/to/target.tar.gz}} {{path/to/file1 path/to/file2 ...}}`

- create a gzipped (compressed) archive from a directory using relative paths:

`tar czf {{path/to/target.tar.gz}} {{[-C|--directory]}} {{path/to/directory}} .`

- Extract a (compressed) archive file into the current directory verbosely:

`tar xvf {{path/to/source.tar.ext}}`

- Extract a (compressed) archive file into the target directory:

`tar xf {{path/to/source.tar.ext}} {{[-C|--directory]}} {{path/to/directory}}`

- create a compressed archive and write it to a file, using the file extension to automatically determine the compression program:

`tar caf {{path/to/target.tar.xz}} {{path/to/file1 path/to/file2 ...}}`

- List the contents of a tar file verbosely:

`tar tvf {{path/to/source.tar}}`

- Extract files matching a pattern from an archive file:

`tar xf {{path/to/source.tar}} --wildcards "{{*.html}}"`
