---
layout: article

type: conference
year: 2020
month: 11

title: 'Grammar-based testing for little languages: an experience report with student compilers'
authors: ['Phillip van Heerden', 'Moeketsi Raselimo', 'Kostis Sagonas', 'Bernd Fischer']

artifact_badges: ['acm_available', 'acm_functional']

DOI:
  target: ACM DL
  id: 10.1145/3426425.3426946


tweet: 'In testing 61 student compilers, we found that no single grammar-based method matched the instructor’s suite, but combining systematic and random suites did better. By adding semantic mark-up tokens to grammars—encoding scope and type constraints—we could automatically generate tests that respect context, match instructor coverage, and expose more real bugs, including in the reference compiler.'

target:
  short: SLE
  full: 'Proceedings of the 13&hairsp;<sup>th</sup> ACM SIGPLAN Conference on Software Languages Engineering, 2020'
  link: 'http://conf.researchr.org/home/sle-2020'

links:
  PDF: '%BASE_URL%/assets/pdf/sle20-little.pdf'
---

###### Abstract

We report on our experience in using various grammar-based test suite generation methods to test 61 
single-pass compilers that undergraduate students submitted for the practical project of a computer architecture course.

We show that (1) all test suites constructed systematically following different grammar coverage 
criteria fall far behind the instructor's test suite in achieved code coverage, in the number of 
triggered semantic errors, and in detected failures and crashes; (2) a medium-sized positive random 
test suite triggers more crashes than the instructor's test suite, but achieves lower code 
coverage and triggers fewer non-crashing errors; and (3) a combination of the systematic and random 
test suites performs as well or better than the instructor's test suite in all aspects and identifies 
errors or crashes in every single submission.

We then develop a light-weight extension of the basic grammar-based testing framework to capture 
contextual constraints, by encoding scoping and typing information as ``semantic mark-up tokens'' 
in the grammar rules. These mark-up tokens are interpreted by a small generic core engine when 
the tests are rendered, and tests with a syntactic structure that cannot be completed into a 
valid program by choosing appropriate identifiers are discarded. 
We formalize individual error models by overwriting individual mark-up tokens, and generate 
tests that are guaranteed to break specific contextual properties of the language. We show that a fully 
automatically generated random test suite with 15 error models achieves roughly the same coverage as 
the instructor's test suite, and outperforms it in the number of triggered semantic errors and 
detected failures and crashes. Moreover, all failing tests indicate real errors, and we 
have detected errors even in the instructor's reference implementation.

###### BibTeX Citation

```bibtex {% raw %}
@inproceedings{DBLP:conf/sle/HeerdenRS020,
  author       = {Phillip van Heerden and
                  Moeketsi Raselimo and
                  Konstantinos Sagonas and
                  Bernd Fischer},
  editor       = {Ralf L{\"{a}}mmel and
                  Laurence Tratt and
                  Juan de Lara},
  title        = {Grammar-based testing for little languages: an experience report with
                  student compilers},
  booktitle    = {Proceedings of the 13th {ACM} {SIGPLAN} International Conference on
                  Software Language Engineering, {SLE} 2020, Virtual Event, USA, November
                  16-17, 2020},
  pages        = {253--269},
  publisher    = {{ACM}},
  year         = {2020},
  url          = {https://doi.org/10.1145/3426425.3426946},
  doi          = {10.1145/3426425.3426946},
  timestamp    = {Sun, 19 Jan 2025 13:25:17 +0100},
  biburl       = {https://dblp.org/rec/conf/sle/HeerdenRS020.bib},
  bibsource    = {dblp computer science bibliography, https://dblp.org}
}
{% endraw %} ```
