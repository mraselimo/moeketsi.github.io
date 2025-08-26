---
layout: article

type: conference
year: 2019
month: 10

title: 'Spectrum-based fault localization for context-free grammars'
authors: ['Moeketsi Raselimo', 'Bernd Fischer']


DOI:
  target: ACM DL
  id: 10.1145/3357766.3359538

tweet: 'New approach to debugging grammars! We present the first spectrum-based fault localization for context-free grammars—ranking suspicious rules via grammar spectra from LL/LR parsers. Evaluated on real & student grammars, it pinpoints faults in up to 40% of cases.'

target:
  short: SLE
  full: 'Proceedings of the 12&hairsp;<sup>th</sup> ACM SIGPLAN Conference on Software Languages Engineering, 2019'
  link: 'http://conf.researchr.org/home/sle-2019'

links:
  PDF: '%BASE_URL%/assets/pdf/sle19-gsbfl.pdf'
---

###### Abstract

We describe and evaluate the first spectrum-based fault localization method aimed at finding faulty rules in a context-free grammar. It takes as input a test suite and a modified parser for the grammar that can collect grammar spectra, i.e., the sets of rules used in attempts to parse the individual test cases, and returns as output a ranked list of suspicious rules. We show how grammar spectra can be collected for both LL and LR parsers, and how the ANTLR and CUP parser generators can be modified and used to automate the collection of the grammar spectra. We evaluate our method over grammars with seeded faults as well as real world grammars and student grammars submitted in compiler engineering courses that contain real faults. The results show that our method ranks the seeded faults within the top five rules in more than half of the cases and can pinpoint them in 10%–40% of the cases. On average, it ranks the faults at around 25% of all rules, and better than 15% for a very large test suite. It also allowed us to identify deviations and faults in the real world and student grammars.

###### BibTeX Citation

```bibtex {% raw %}
@inproceedings{DBLP:conf/sle/RaselimoF19,
  author       = {Moeketsi Raselimo and
                  Bernd Fischer},
  editor       = {Oscar Nierstrasz and
                  Jeff Gray and
                  Bruno C. d. S. Oliveira},
  title        = {Spectrum-based fault localization for context-free grammars},
  booktitle    = {Proceedings of the 12th {ACM} {SIGPLAN} International Conference on
                  Software Language Engineering, {SLE} 2019, Athens, Greece, October
                  20-22, 2019},
  pages        = {15--28},
  publisher    = {{ACM}},
  year         = {2019},
  url          = {https://doi.org/10.1145/3357766.3359538},
  doi          = {10.1145/3357766.3359538},
  timestamp    = {Mon, 21 Jun 2021 12:26:17 +0200},
  biburl       = {https://dblp.org/rec/conf/sle/RaselimoF19.bib},
  bibsource    = {dblp computer science bibliography, https://dblp.org}
}
{% endraw %} ```
