---
layout: article

type: thesis
year: 2023
month: 3

title: 'Fault Localization and Repair for Grammarware'
authors: ['Moeketsi Raselimo']

target:
  short: 'PhD Dissertation'

links:
  PDF: '%BASE_URL%/assets/pdf/thesis.pdf'
---

###### Abstract
Context-free grammars describe the formal structure of
complex texts, such as PDF documents, configuration files
or computer programs. However, grammar bugs can cause
the software systems processing these texts to fail. This
study develops a fully automatic approach to find and fix
grammar bugs using only a given set of passing and failing
tests, the grammar and the executable system. It identifies
fault locations through the execution differences between
the passing and failing tests and incrementally patches the
faults using small-scale grammar transformations. It finds
bugs in production grammars and fixes grammars written
by students in a postgraduate compiler course.

###### BibTeX Citation

```bibtex {% raw %}
@phdthesis{stellies23/raselimo,
  title   = {Fault Localization and Repair for Grammarware},
  author  = {Moeketsi Raselimo},
  year    = {2023},
  school  = {Stellenbosch University}
}
{% endraw %} ```
