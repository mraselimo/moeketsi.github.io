---
layout: article

type: conference
year: 2020
month: 11

title: 'An interactive feedback system for grammar development (tool paper)'
authors: ['Chelsea Barraball', 'Moeketsi Raselimo',  'Bernd Fischer']

artifact_badges: ['acm_available', 'acm_functional']

DOI:
  target: ACM DL
  id: 10.1145/3426425.3426935


tweet: 'gtutr: an interactive feedback system for learning context-free grammars with ANTLR. It clusters failing tests via sequence alignment, avoids overload, adds light gamification, and visualizes progress—helping students debug smarter, not harder.'

target:
  short: SLE
  full: 'Proceedings of the 13&hairsp;<sup>th</sup> ACM SIGPLAN Conference on Software Languages Engineering, 2020'
  link: 'http://conf.researchr.org/home/sle-2020'

links:
  PDF: '%BASE_URL%/assets/pdf/sle20-gtutr.pdf'
---

###### Abstract
We describe gtutr, an interactive feedback system designed to assist students in developing context-free grammars and corresponding ANTLR parsers. It intelligently controls students' access to a large test suite for the target language. After each submission, gtutr analyzes any failing tests and uses the Needleman-Wunsch sequence alignment algorithm over the tests' rule traces to identify and eliminate similar failing tests. This reduces the redundancy in the feedback given to the students and prevents them from being overloaded. gtutr uses simple gamification to encourage independent problem solving by students: it gives as little information as possible, and students need to prompt the system for further details such as failing tests similar to or different from already seen tests, or even for hints about rules that are the most likely to contain faults. It tracks the students' information requests and uses this to attenuate marks following an instructor-set penalty schema. The system also visualizes test outcomes over multiple submissions, helping students to keep track of the effects of their changes as their grammar development progresses.

###### BibTeX Citation

```bibtex {% raw %}
@inproceedings{DBLP:conf/sle/BarraballR020,
  author       = {Chelsea Barraball and
                  Moeketsi Raselimo and
                  Bernd Fischer},
  editor       = {Ralf L{\"{a}}mmel and
                  Laurence Tratt and
                  Juan de Lara},
  title        = {An interactive feedback system for grammar development (tool paper)},
  booktitle    = {Proceedings of the 13th {ACM} {SIGPLAN} International Conference on
                  Software Language Engineering, {SLE} 2020, Virtual Event, USA, November
                  16-17, 2020},
  pages        = {101--107},
  publisher    = {{ACM}},
  year         = {2020},
  url          = {https://doi.org/10.1145/3426425.3426935},
  doi          = {10.1145/3426425.3426935},
  timestamp    = {Sat, 08 Jan 2022 02:24:28 +0100},
  biburl       = {https://dblp.org/rec/conf/sle/BarraballR020.bib},
  bibsource    = {dblp computer science bibliography, https://dblp.org}
}
{% endraw %} ```
