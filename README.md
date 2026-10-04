# tldr-pages — English common pages (scoped mirror)

Mirror of [tldr-pages/tldr](https://github.com/tldr-pages/tldr) scoped to
`pages/common/**` — the ~4,700 English command pages. The full upstream
repository carries ~30k pages across dozens of locale trees plus client
specification and governance docs; for retrieval corpora the locale
duplicates crowd the English pages out of the top hits (measured: a
5-query pre-registered G7 suite returned 2/5 relevant on the full repo
versus multilingual duplicates outranking the target pages).

Pinned upstream commit: b328cc85bbe021e4d815941a77049eda633b1ec9
Licence: CC-BY-4.0 (LICENSE.md, upstream) — unchanged by this scoping.
Rebuilt by the XERJ Corpus Hub program; regeneration is
`git clone upstream && cp -r pages/common .` at a new commit.

## Retrieval normalisation (2026-10-04)

tldr's client convention bolds one focal letter by bracketing it —
`e[x]ecute`, `[u]ser`, `[e]dit` — which render engines display as bold but
which shred the token in a lexical index (`execute` never forms; the token
stream sees `e`/`x`/`ecute`). Measured on the pre-registered G7 suite
`g7-tonight-2026-10`: a query phrased "give the owner of a file permission
to execute it" could not match `chmod u+x`'s description because every key
word was bracket-split (`match body:execute` → 140 docs, not chmod.md;
`match body:ecute` → exactly chmod.md).

This mirror normalises that convention away: every single-letter bracket
pair (`[x]`) is unbracketed to the bare letter (785 occurrences across the
tree; zero markdown links affected — verified `\[([A-Za-z])\]` never
precedes `(`). No other text is altered; pages remain verbatim otherwise.
Regeneration adds: `find pages -name '*.md' -exec sed -Ei 's/\[([A-Za-z])\]/\1/g' {} +`
