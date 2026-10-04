# ar

> Create, modify, and extract from Unix archives. Typically used for static libraries (`.a`) and Debian packages (`.deb`).
> See also: `tar`.
> More information: <https://manned.org/ar>.

- Extract all members from an archive:

`ar x {{path/to/file.a}}`

- List contents in a specific archive:

`ar t {{path/to/file.ar}}`

- replace or add specific files to an archive:

`ar r {{path/to/file.deb}} {{path/to/debian-binary path/to/control.tar.gz path/to/data.tar.xz ...}}`

- Insert an object file index (equivalent to using `ranlib`):

`ar s {{path/to/file.a}}`

- Create an archive with specific files and an accompanying object file index:

`ar rs {{path/to/file.a}} {{path/to/file1.o path/to/file2.o ...}}`
