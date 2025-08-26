---
layout: article

type: workshop
year: 2025
month: 04

title: 'Which Inputs Trigger my Patch?'
authors: ['Martin Eberlein', 'Moeketsi Raselimo', 'Lars Grunske']

DOI:
  target: IEEE
  id: 10.1109/APR66717.2025.00006

tweet: 'Automated Program Repair is powerful, but can devs trust the fixes?
We present AVICENNAPATCH: a tool that explains what inputs a patch actually fixes using differential testing + grammar-based constraints.
More transparency, better trust in APR!'

target:
  short: APR @ ICSE
  full: 'IEEE/ACM International Workshop on Automated Program Repair'
  link: 'https://program-repair.org/workshop-2025/'

links:
  PDF: '%BASE_URL%/assets/pdf/2025APR-PatchAvicenna.pdf'
---

###### Abstract
Automated program repair (APR) has made significant progress in autonomously locating and fixing software faults.
However, developers face uncertainty in trusting and validating
patches, as the boundaries of the patch and the concrete inputs
the patch fixes often remain unclear.
In this paper, we introduce AVICENNAPATCH, a novel tool designed to provide precise explanations of the input structures that
are covered by the patch. Building on the AVICENNA framework,
AVICENNAPATCH uses a differential testing strategy, executing
both the original and patched program versions to identify
inputs where behavior diverges. By leveraging ISLA constraints,
AVICENNAPATCH generates human-readable, grammar-based
explanations that characterize patch-triggering inputs in terms
of syntactic and semantic features. To refine these explanations,
AVICENNAPATCH iteratively generates new inputs and adjusts its
hypotheses, ensuring that the explanations are both precise and
generalizable. Our approach not only enhances transparency in
APR by clarifying the operational boundaries of patches but also
supports developers in evaluating the reliability and robustness of
automated fixes across diverse input scenarios. Our evaluation on
12 patches for 7 different subjects shows that AVICENNAPATCH
can provide effective and general explanations.
###### BibTeX Citation

```bibtex {% raw %}
@inproceedings{DBLP:conf/icse-apr/EberleinRG25,
  author       = {Martin Eberlein and
                  Moeketsi Raselimo and
                  Lars Grunske},
  title        = {Which Inputs Trigger My Patch?},
  booktitle    = {{IEEE/ACM} International Workshop on Automated Program Repair, APR@ICSE
                  2025, Ottawa, ON, Canada, April 29, 2025},
  pages        = {3--10},
  publisher    = {{IEEE}},
  year         = {2025},
  url          = {https://doi.org/10.1109/APR66717.2025.00006},
  doi          = {10.1109/APR66717.2025.00006},
  timestamp    = {Mon, 30 Jun 2025 21:48:33 +0200},
  biburl       = {https://dblp.org/rec/conf/icse-apr/EberleinRG25.bib},
  bibsource    = {dblp computer science bibliography, https://dblp.org}
}
{% endraw %} ```
