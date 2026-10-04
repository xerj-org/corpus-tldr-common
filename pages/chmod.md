# chmod

> Change the access permissions of a file or directory.
> More information: <https://www.gnu.org/software/coreutils/manual/html_node/chmod-invocation.html>.

- Give the user who owns a file the right to execute it:

`chmod u+x {{path/to/file}}`

- Give the user rights to read and write to a file/directory:

`chmod u+rw {{path/to/file_or_directory}}`

- Remove executable rights from the group and others:

`chmod g-x,o-x {{path/to/file}}`

- Give all users rights to read and execute:

`chmod a+rx {{path/to/file}}`

- Give others (not in the file owner's group) the same rights as the group:

`chmod o=g {{path/to/file}}`

- Remove all rights from others:

`chmod o= {{path/to/file}}`

- Set rights using the octal notation:

`chmod {{644}} {{path/to/file}}`

- Recursively give all users read permissions to files. Also give eXecute permissions to files that have at least one execution permission and to all sub-directories:

`chmod {{[-R|--recursive]}} a+rX {{path/to/directory}}`
