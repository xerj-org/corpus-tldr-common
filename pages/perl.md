# perl

> The Perl 5 language interpreter.
> See also: `perldoc`.
> More information: <https://perldoc.perl.org/perl>.

- Print lines from `stdin` matching `regex1` and case insensitive `regex2`:

`perl -n -e 'print if m/regex1/ and m/regex2/i'`

- Say ([-E]) first match group, using a `regex`, ignoring space (x) in `regex`:

`perl -n -E 'say $1 if m/{{before}} ( {{group_regex}} ) {{after}}/x'`

- in-place, with backup, substitute all occurrence (g) of `regex` with a replacement:

`perl -i'.bak' -p -e 's/regex/{{replacement}}/g' {{path/to/files}}`
