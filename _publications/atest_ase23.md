---
layout: article

type: workshop
year: 2023
month: 10

title: 'Static Test Case Prioritization Strategies for Grammar-Based Testing'
authors: ['Moeketsi Raselimo', 'Lars Grunske', 'Bernd Fischer']

DOI:
  target: IEEE
  id: 10.1109/ASEW60602.2023.00025

tweet: 'Grammar-based test generators can produce huge suites, but running them is costly. We show that simple prioritization strategies (e.g., input length, novel rule coverage, rule frequency) can improve fault detection vs. random ordering—though performance varies across suites.'

target:
  short: ATest @ ASE
  full: '2023 38th IEEE/ACM International Conference on Automated Software Engineering Workshops (ASEW)'
  link: 'https://conf.researchr.org/track/ase-2023/ase-2023--workshop--a-test?'

links:
  PDF: '%BASE_URL%/assets/pdf/atest_ase23.pdf'
---

###### Abstract
Grammar-based test case generators can quickly produce large test suites that structurally and systematically cover the input space of a system under test. However, running these large test suites requires large computation resources. In this paper, we investigate whether simple test case prioritization strategies based on statically determined grammar-related properties (e.g., token-length of input, novel rule coverage, and relative frequency of rule coverage), can detect faults in the system under test faster. Our preliminary results indicate that different test execution orderings from these strategies have an effect on the fault detection rate. Their performance varies across the different test suites, but they generally perform better than a simple random ordering of test executions.

###### BibTeX Citation

```bibtex {% raw %}
@inproceedings{DBLP:conf/kbse/RaselimoGF23,
  author       = {Moeketsi Raselimo and
                  Lars Grunske and
                  Bernd Fischer},
  title        = {Static Test Case Prioritization Strategies for Grammar-Based Testing},
  booktitle    = {38th {IEEE/ACM} International Conference on Automated Software Engineering,
                  {ASE} 2023 - Workshops, Luxembourg, September 11-15, 2023},
  pages        = {151--158},
  publisher    = {{IEEE}},
  year         = {2023},
  url          = {https://doi.org/10.1109/ASEW60602.2023.00025},
  doi          = {10.1109/ASEW60602.2023.00025},
  timestamp    = {Thu, 16 Nov 2023 09:03:51 +0100},
  biburl       = {https://dblp.org/rec/conf/kbse/RaselimoGF23.bib},
  bibsource    = {dblp computer science bibliography, https://dblp.org}
}
{% endraw %} ```
