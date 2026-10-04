# ipcs

> Show information about the usage of XSI IPC facilities: shared memory segments, message queues, and semaphore arrays.
> More information: <https://manned.org/ipcs.1p>.

- Show information about all the IPC:

`ipcs -a`

- Show information about active shared memory segments, message queues or semaphore sets:

`ipcs {{-m|-q|-s}}`

- Show information on maximum allowable size in bytes:

`ipcs -b`

- Show creator's user name and group name for all IPC facilities:

`ipcs -c`

- Show the pID of the last operators for all IPC facilities:

`ipcs -p`

- Show access times for all IPC facilities:

`ipcs -t`

- Show outstanding usage for active message queues, and shared memory segments:

`ipcs -o`
