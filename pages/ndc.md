# ndc

> Name daemon control service for name servers.
> If a command isn't provided, NDC will prompt for one until EOF.
> More information: <https://manned.org/ndc>.

- Set the control channel rendezvous point:

`ndc -c {{channel}} {{command}}`

- Bind the client side to a specific localsock address:

`ndc -l {{localsock}} {{command}}`

- Set path to pidfile for UNIX signal control:

`ndc -p {{path/to/pidfile}} {{command}}`

- Enable debugging:

`ndc -d {{command}}`

- Enable quiet mode:

`ndc -q {{command}}`

- Enable nonfatal error suppression:

`ndc -s {{command}}`

- Enable tracing for protocol and system debugging:

`ndc -t {{command}}`

- List built-in commands:

`ndc /help`
