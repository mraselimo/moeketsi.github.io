---
layout: article

type: conference
year: 2026
month: 10

title: 'Learning the Lexical Structure of Black-Box Systems by Parsing Systematic String Edit Mutations'
authors: ['Moeketsi Raselimo', 'Lars Grunske', 'Bernd Fischer']

DOI:
  target: ACM DL
  id: 10.1145/3832783.3834391

awards:
  - icon: star
    desc: 'ACM SIGSOFT Distinguished Paper Award'

tweet: 'We learn the lexical structure of black-box systems by systematically mutating valid input strings and generalizing from membership-query responses. The learned tokens can serve as lexer test oracles and improve downstream grammar learning.'

target:
  short: ASE
  full: 'Proceedings of the 41&hairsp;<sup>st</sup> IEEE/ACM International Conference on Automated Software Engineering, 2026'
  link: 'https://conf.researchr.org/home/ase-2026'

links:
  PDF: '%BASE_URL%/assets/pdf/ase26_lexinfer.pdf'
---

###### Abstract

We describe and evaluate an approach to learn the lexical structure of black-box systems from a set of positive training examples. Our core idea is to use the system as oracle for repeated membership queries which we construct by systematically mutating the training examples using different string edit operations. We then learn the elements of the lexical structure by generalizing from the oracle responses to the mutated training examples.

We have applied this approach to several systems with target languages of varying complexity, such as TinyC, JSON, AMPL, Modula-2, Oberon, Zig, or C. We show that the learned tokens are similar, and in many cases identical, to those of the oracle lexers. Their inspection can indicate where the systems under test deviate from the lexical structure of their respective target languages; the learned tokens can thus serve as precise test oracles for lexers. We show that the segmentations induced by lexing the validation sets with the learned and oracle lexers, respectively, are identical in many cases and that the non-identical parts affect on average between zero and about 15 percent of the characters. We finally demonstrate that using the learned tokens substantially improves the quality of the context-free grammar that the state-of-the-art grammar learner Kedavra learns for cJSON, increasing the average F1-score of the grammars learned in five runs from 0.93 to 1.00.

###### BibTeX Citation

```bibtex {% raw %}
@inproceedings{RaselimoGF26,
  author       = {Moeketsi Raselimo and
                  Lars Grunske and
                  Bernd Fischer},
  title        = {Learning the Lexical Structure of Black-Box Systems by Parsing
                  Systematic String Edit Mutations},
  booktitle    = {Proceedings of the 41st {IEEE/ACM} International Conference on
                  Automated Software Engineering, {ASE} 2026, Munich, Germany,
                  October 12-16, 2026},
  pages        = {764--776},
  publisher    = {{ACM}},
  year         = {2026},
  url          = {https://doi.org/10.1145/3832783.3834391},
  doi          = {10.1145/3832783.3834391}
}
{% endraw %} ```
