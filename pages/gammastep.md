# gammastep

> Adjust the screen's color temperature according to the time of day.
> See also: `redshift`.
> More information: <https://manned.org/gammastep>.

- Turn on Gammastep with temperature set to 5700k during the day and 3600k at night:

`gammastep -t 5700:3600`

- Turn on Gammastep with a manually specified custom location:

`gammastep -l {{latitude}}:{{longitude}}`

- Turn on Gammastep with screen brightness set to 70% during the day and 40% at night:

`gammastep -b 0.7:0.4`

- Turn on Gammastep with custom gamma levels (between 0 and 1):

`gammastep -g {{red}}:{{green}}:{{blue}}`

- Turn on Gammastep with a cOnstant unchanging color temperature:

`gammastep -O {{temperature}}`

- Reset temperature adjustments applied by Gammastep:

`gammastep -x`
