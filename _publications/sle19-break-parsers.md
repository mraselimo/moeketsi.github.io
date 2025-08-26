---
layout: article

type: conference
year: 2019
month: 10

title: 'Breaking parsers: mutation-based generation of programs with guaranteed syntax errors'
authors: ['Moeketsi Raselimo', 'Jan Taljaard', 'Bernd Fischer']


DOI:
  target: ACM DL
  id: 10.1145/3357766.3359542

awards:
  - icon: star
    desc: 'ACM SIGPLAN Distinguished Paper'

tweet: 'We explore two mutation-based methods for generating programs with guaranteed 
    syntax errors — word mutation (token edits) and rule mutation (grammar edits) — to 
    complement traditional grammar-based testing focused only on valid programs.'

target:
  short: SLE
  full: 'Proceedings of the 12&hairsp;<sup>th</sup> ACM SIGPLAN Conference on Software Languages Engineering, 2019'
  link: 'http://conf.researchr.org/home/sle-2019'

links:
  PDF: '%BASE_URL%/assets/pdf/sle19-break.pdf'
---

###### Abstract

Grammar-based test case generation has focused almost exclusively on generating 
syntactically correct programs (i.e., positive tests) from a context-free reference 
grammar but a positive test suite cannot detect when the unit under test 
accepts words outside the language (i.e., false positives). Here, we 
investigate the converse problem and describe two mutation-based approaches 
for generating programs with guaranteed syntax errors (i.e., negative tests). 
Word mutation systematically modifies positive tests by deleting, inserting, substituting, 
and transposing tokens in such a way that at least one impossible token pair emerges. 
Rule mutation applies such operations to the symbols of the right-hand sides 
of productions in such a way that 
each derivation that uses the mutated rule yields a word outside the language.

###### BibTeX Citation

```bibtex {% raw %}
@inproceedings{DBLP:conf/sle/RaselimoTF19,
  author       = {Moeketsi Raselimo and
                  Jan Taljaard and
                  Bernd Fischer},
  editor       = {Oscar Nierstrasz and
                  Jeff Gray and
                  Bruno C. d. S. Oliveira},
  title        = {Breaking parsers: mutation-based generation of programs with guaranteed
                  syntax errors},
  booktitle    = {Proceedings of the 12th {ACM} {SIGPLAN} International Conference on
                  Software Language Engineering, {SLE} 2019, Athens, Greece, October
                  20-22, 2019},
  pages        = {83--87},
  publisher    = {{ACM}},
  year         = {2019},
  url          = {https://doi.org/10.1145/3357766.3359542},
  doi          = {10.1145/3357766.3359542},
  timestamp    = {Sun, 19 Jan 2025 13:25:16 +0100},
  biburl       = {https://dblp.org/rec/conf/sle/RaselimoTF19.bib},
  bibsource    = {dblp computer science bibliography, https://dblp.org}
}
{% endraw %} ```
