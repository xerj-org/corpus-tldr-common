# wondershaper

> Allow the user to limit the bandwidth of network adapters.
> More information: <https://github.com/magnific0/wondershaper#usage>.

- Show the current status of a specific adapter:

`wondershaper -s -a {{adapter_name}}`

- Clear limits from a specific adapter:

`wondershaper -c -a {{adapter_name}}`

- Set a specific maximum download rate (in Kbps):

`wondershaper -a {{adapter_name}} -d {{1024}}`

- Set a specific maximum upload rate (in Kbps):

`wondershaper -a {{adapter_name}} -u {{512}}`

- Set a specific maximum download rate and upload rate (in Kbps):

`wondershaper -a {{adapter_name}} -d {{1024}} -u {{512}}`

- Display help:

`wondershaper -h`
