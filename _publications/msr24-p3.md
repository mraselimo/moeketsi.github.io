---
layout: article

type: conference
year: 2024
month: 04

title: 'P3: A Dataset of Partial Program Fixes'
authors: ['Dirk Beyer', 'Lars Grunske', 'Matthias Kettl', 'Marian Lingsch-Rosenfeld', 'Moeketsi Raselimo']

artifact_badges: ['acm_available', 'acm_functional', 'acm_reusable']

DOI:
  target: ACM DL
  id: 10.1145/3643991.3644889

tweet: 'New dataset for the SE community: P3—a curated collection of incomplete bug fixes from real-world C projects. Each case documents multiple partial fixes leading to a complete fix, enabling reproducible studies on patch correctness, fix evolution, and automated repair.'

target:
  short: MSR
  full: 'Proceedings of the 21&hairsp;<sup>st</sup> Internation Conference on Mining Software Repositories, 2024'
  link: 'https://2024.msrconf.org/'

links:
  PDF: '%BASE_URL%/assets/pdf/msr24-p3.pdf'
---

###### Abstract
Identifying and fixing bugs in programs remains a challenge and is one of the most time-consuming tasks in software development. But even after a bug is identified, and a fix has been proposed by a developer or tool, it is not uncommon that the fix is incomplete and does not cover all possible inputs that trigger the bug. This can happen quite often and leads to re-opened issues and inefficiencies. In this paper, we introduce P3, a curated dataset composed of incomplete fixes. Each entry in the set contains a series of commits fixing the same underlying issue, where multiple of the intermediate commits are incomplete fixes. These are sourced from real-world open-source C projects. The selection process involves both automated and manual stages. Initially, we employ heuristics to identify potential partial fixes from repositories, subsequently we validate them through meticulous manual inspection. This process ensures the accuracy and reliability of our curated dataset. We envision that the dataset will support researchers while investigating partial fixes in more detail, allowing them to develop new techniques to detect and fix them. We make our dataset publicly available at https://gitlab.com/sosy-lab/research/data/partial-fix-dataset.

###### BibTeX Citation

```bibtex {% raw %}
@inproceedings{DBLP:conf/msr/BeyerGKRR24,
  author       = {Dirk Beyer and
                  Lars Grunske and
                  Matthias Kettl and
                  Marian Lingsch Rosenfeld and
                  Moeketsi Raselimo},
  editor       = {Diomidis Spinellis and
                  Alberto Bacchelli and
                  Eleni Constantinou},
  title        = {{P3:} {A} Dataset of Partial Program Patches},
  booktitle    = {21st {IEEE/ACM} International Conference on Mining Software Repositories,
                  {MSR} 2024, Lisbon, Portugal, April 15-16, 2024},
  pages        = {123--127},
  publisher    = {{ACM}},
  year         = {2024},
  url          = {https://doi.org/10.1145/3643991.3644889},
  doi          = {10.1145/3643991.3644889},
  timestamp    = {Thu, 22 Aug 2024 20:23:18 +0200},
  biburl       = {https://dblp.org/rec/conf/msr/BeyerGKRR24.bib},
  bibsource    = {dblp computer science bibliography, https://dblp.org}
}
{% endraw %} ```
