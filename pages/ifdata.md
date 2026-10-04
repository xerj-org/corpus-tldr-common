# ifdata

> Display information about a network interface.
> More information: <https://manned.org/ifdata>.

- print the whole configuration of the specified interface:

`ifdata -p {{eth0}}`

- Indicate the existence of the specified interface via the exit code:

`ifdata -e {{eth0}}`

- print the IPv4 address and the netmask of the specified interface:

`ifdata -pa -pn {{eth0}}`

- print the Network address, the broadcast address, and the mTU of the specified interface:

`ifdata -pN -pb -pm {{eth0}}`

- Display help:

`ifdata`
