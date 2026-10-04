# cfv

> Command-line File Verify, a utility to test and create checksum files.
> More information: <https://manned.org/cfv>.

- Test checksum files in current directory:

`cfv -T`

- Test verbosely, rename bad, and show unverified files using a checksum file:

`cfv -Tvnu -f {{path/to/file}}`

- Create a checksum file of a specific type for the selected files:

`cfv -C -t "{{sfv|sha256|md5|...}}" {{file1 file2 ...}}`

- Create separate checksum files for each recursively selected directory:

`cfv -Cr`

- Create a single `sha256` type file for all [rr]ecursively selected files:

`cfv -C -f {{sums.sha256}} -rr`

- Create a `gzipped` `.sfv` file verbosely, following `symlinks` and using `path/to/directory` as base path:

`cfv -Czvl -p {{path/to/directory}}`
