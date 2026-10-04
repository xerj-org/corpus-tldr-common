# babeld

> Routing daemon for Babel which uses firewall-style filters.
> More information: <https://www.irif.fr/~jch/software/babel/babeld.html>.

- Start the daemon with one or more configuration files (read in order):

`babeld -c {{path/to/ports.conf}} -c {{path/to/filters.conf}} -c {{path/to/interfaces.conf}}`

- Daemonize after startup:

`babeld -D`

- Specify a Configuration command:

`babeld -C '{{redistribute metric 256}}'`

- Specify on which interfaces to operate:

`babeld {{eth0}} {{eth1}} {{wlan0}}`
