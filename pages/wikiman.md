# wikiman

> Offline search engine for documentation.
> Supports manual pages, Arch Wiki, Gentoo Wiki, FreeBSD documentation, and tldr-pages.
> More information: <https://github.com/filiparag/wikiman#usage>.

- Search for a specific topic in all installed sources:

`wikiman {{search_term}}`

- Search for a topic in a specific source:

`wikiman -s {{source}} {{search_term}}`

- Search for a topic in two or more specific sources:

`wikiman -s {{source1,source2,...}} {{search_term}}`

- List existing Sources:

`wikiman -S`

- Display help:

`wikiman -h`
