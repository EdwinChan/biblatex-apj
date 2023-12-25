Probably the first `biblatex` style compatible with the bibliography and
citation styles of The Astrophysical Journal. [Multiple
preprints](https://arxiv.org/a/0000-0001-5949-6109) use this style.

Bibliography options can be enabled with
`\ExecuteBibliographyOptions{<option>, <option>, …}`.
Available `<option>`s are:

* `embedlinks`: Embed hyperlinks into the journal, volume, and page of each
  bibliography item that link to the webpages indicated by the `doi`,
  `bibcode`, and `eprint` fields, respectively, of the bibliography entry.
  Embedding does not occur at all if the package `hyperref` is not loaded,
  embedding of individual links does not occur if the corresponding fields are
  missing, and embedding of the arXiv link does not occur if the `eprinttype`
  field is not equal to `"arXiv"`. DOI and arXiv links that are not embedded
  appear at the end of each bibliography item; ADS links are simply omitted.

* `doilinkcolor=<color>`: Set the color of embedded DOI links. `<color>` can be
  in any format accepted by `\hypersetup{urlcolor=<color>}`.

* `adslinkcolor=<color>`: Set the color of embedded ADS links.

* `arxivlinkcolor=<color>`: Set the color of embedded arXiv links.

* `numeric`: Number bibliography items. This does not affect the citation
  style.

To make the dashes for repeated authors longer, add
`\setlength\bibhang{1.25em}` before `\printbibliography`.
