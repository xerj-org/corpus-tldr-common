# argon2

> Calculate Argon2 cryptographic hashes.
> More information: <https://github.com/P-H-C/phc-winner-argon2#command-line-utility>.

- Calculate a hash with a password and a salt with the default parameters:

`echo "{{password}}" | argon2 "{{salt_text}}"`

- Calculate a hash with the specified algorithm:

`echo "{{password}}" | argon2 "{{salt_text}}" -{{d|i|id}}`

- Display the output encoded hash without additional information:

`echo "{{password}}" | argon2 "{{salt_text}}" -e`

- Calculate a hash with given iteration times, memory usage, and parallelism parameters:

`echo "{{password}}" | argon2 "{{salt_text}}" -t {{5}} -m {{20}} -p {{7}}`
