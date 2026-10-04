# certutil

> Manage keys and certificates in both NSS databases and other NSS tokens.
> More information: <https://manned.org/certutil>.

- Create a New certificate database in the current directory:

`certutil -N -d .`

- List all certificates in a database:

`certutil -L -d .`

- List all private Keys in a database specifying the password file:

`certutil -K -d . -f {{path/to/password_file.txt}}`

- Add the signed certificate to the requesters database specifying a nickname, trust attributes and an input CRT file:

`certutil -A -n "{{server_certificate}}" -t ",," -i {{path/to/file.crt}} -d .`

- Add subject alternative names to a given certificate with a specific key size (g):

`certutil -S -f {{path/to/password_file.txt}} -d . -t ",," -c "{{server_certificate}}" -n "{{server_name}}" -g {{2048}} -s "CN={{common_name}},O={{organization}}"`
