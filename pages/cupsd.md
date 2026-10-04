# cupsd

> Server daemon for the CUPS print server.
> More information: <https://openprinting.github.io/cups/doc/man-cupsd.html>.

- Start `cupsd` in the background, aka. as a daemon:

`cupsd`

- Start `cupsd` on the foreground:

`cupsd -f`

- launch `cupsd` on-demand (commonly used by `launchd` or `systemd`):

`cupsd -l`

- Start `cupsd` using the specified `cupsd.conf` configuration file:

`cupsd -c {{path/to/cupsd.conf}}`

- Start `cupsd` using the specified `cups-files.conf` configuration file:

`cupsd -s {{path/to/cups-files.conf}}`

- test the `cupsd.conf` configuration file for errors:

`cupsd -t -c {{path/to/cupsd.conf}}`

- test the `cups-files.conf` configuration file for errors:

`cupsd -t -s {{path/to/cups-files.conf}}`

- Display help:

`cupsd -h`
