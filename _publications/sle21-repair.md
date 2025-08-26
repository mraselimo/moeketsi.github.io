---
layout: article

type: conference
year: 2021
month: 10

title: 'Automatic grammar repair'
authors: ['Moeketsi Raselimo', 'Bernd Fischer']


DOI:
  target: ACM DL
  id: 10.1145/3486608.3486910

tweet: 'Meet gfixr: the first system to automatically repair context-free grammars. Using spectrum-based fault localization + targeted patches, it iteratively fixes faulty rules until all tests pass—shown effective on student grammars & even Pascal dialects.'

target:
  short: SLE
  full: 'Proceedings of the 14&hairsp;<sup>th</sup> ACM SIGPLAN Conference on Software Languages Engineering, 2021'
  link: 'http://conf.researchr.org/home/sle-2021'

links:
  PDF: '%BASE_URL%/assets/pdf/sle21-repair.pdf'
---

###### Abstract

We describe the first approach to automatically repair bugs in context-free grammars: given a grammar that fails some tests in a given test suite, we iteratively and gradually transform the grammar until it passes all tests. Our core idea is to build on spectrum-based fault localization to identify promising repair sites (i.e., specific positions in rules), and to apply grammar patches at these sites whenever they satisfy explicitly formulated pre-conditions necessary to potentially improve the grammar.

We have implemented this approach in the gfixr system, and successfully used it to fix grammars students submitted as homeworks in a compiler engineering course, and to map one Pascal dialect grammar against another dialect. gfixr can be configured to explore the repair space in different ways, and can also take advantage of counterexamples to enable restriction patches that make the grammar less permissive.
###### BibTeX Citation

```bibtex {% raw %}
@inproceedings{DBLP:conf/sle/Raselimo021,
  author       = {Moeketsi Raselimo and
                  Bernd Fischer},
  editor       = {Eelco Visser and
                  Dimitris S. Kolovos and
                  Emma S{\"{o}}derberg},
  title        = {Automatic grammar repair},
  booktitle    = {{SLE} '21: 14th {ACM} {SIGPLAN} International Conference on Software
                  Language Engineering, Chicago, IL, USA, October 17 - 18, 2021},
  pages        = {126--142},
  publisher    = {{ACM}},
  year         = {2021},
  url          = {https://doi.org/10.1145/3486608.3486910},
  doi          = {10.1145/3486608.3486910},
  timestamp    = {Sat, 08 Jan 2022 02:24:28 +0100},
  biburl       = {https://dblp.org/rec/conf/sle/Raselimo021.bib},
  bibsource    = {dblp computer science bibliography, https://dblp.org}
}
{% endraw %} ```
