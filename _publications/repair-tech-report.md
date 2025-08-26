---
layout: article

type: report
year: 2023
month: 4

title: 'Passive and Active Automatic Grammar Repair'
authors: ['Moeketsi Raselimo', 'Bernd Fischer']

target:
  short: 'SSRN' 
  link: 'http://sygus.org/comp/2018'

links:
  PDF: '%BASE_URL%/assets/pdf/repair-tech-report.pdf'
---

###### Abstract
We describe the first approach to automatically repair faults in context-free grammars: given a grammar that fails some tests in a test suite, we iteratively and gradually transform the grammar until it passes all tests. Our core idea is to use spectrum-based fault localization to identify promising repair sites (ie, specific positions in rules), and to apply grammar patches at these sites whenever they satisfy explicitly formulated pre-conditions necessary to potentially improve the grammar. We implement and evaluate a passive and an active variant of our repair approach. In passive repair, we repair against the fixed input test suite as specification. The key extension of the active repair is to exploit an oracle in the form of a black-box parser for the target language to incorporate a test suite enrichment into the repair. This generates additional tests from each repair candidate and issues membership queries to the oracle to confirm the outcome of each of these tests. We demonstrate the effectiveness of both repair variants using thirty-three student grammars that contain multiple real faults. We show that both variants are effective in fixing real faults in these grammars but that active repair produces repairs with higher precision than passive repair.
###### BibTeX Citation

```bibtex {% raw %}
@misc{RaselimoFischer2023GrammarRepair,
  title        = {Passive and Active Automatic Grammar Repair},
  author       = {Raselimo, Moeketsi and Fischer, Bernd},
  year         = {2023},
  month        = apr,
  note         = {SSRN working paper},
  doi          = {10.2139/ssrn.4421956},
  url          = {https://ssrn.com/abstract=4421956}
}

{% endraw %} ```
