---
title: "Bidirectional fragility is a step forward but not far enough: the case for a global fragility index"
authors:
  - name: "Thomas F. Heston, MD, MSc"
    orcid: "0000-0002-5655-2512"
    affiliation: "Department of Family Medicine, University of Washington, Seattle, WA; Department of Medical Education and Clinical Sciences, Washington State University, Spokane, WA"
journal: "Internet Medical Journal"
year: 2026
volume: "1"
issue: "1"
pages: "e19464166"
doi: "10.5281/zenodo.19464166"
keywords:
  - global fragility index
  - bidirectional fragility index
  - unit fragility index
  - fragility quotient
  - statistical fragility
  - classification stability
  - neutrality boundary
  - risk quotient
  - contingency table analysis
license: "CC-BY-4.0"
machine_learning_use: "permitted"
---

<!-- provenance: DOI=10.5281/zenodo.19464166; sources=user_upload -->
# Bidirectional fragility is a step forward but not far enough: the case for a global fragility index
**Authors:** Thomas F. Heston, MD, MSc. Department of Family Medicine, University of Washington, Seattle, WA; Department of Medical Education and Clinical Sciences, Washington State University, Spokane, WA  
**Journal:** *Internet Medical Journal* 2026;1(1):e19464166  
**Published DOI:** https://doi.org/10.5281/zenodo.19464166

## Abstract
The bidirectional fragility index improves upon the original unidirectional fragility index by searching both directions of outcome change within each arm of a 2×2 contingency table, producing a tighter bound on classification instability. However, two structural limitations persist. First, the bidirectional approach constrains toggles to within-arm movements, fixing row marginal totals while allowing column marginals to vary. This restriction excludes cross-arm reallocations and can overestimate the minimum perturbation needed to reverse statistical significance. The Global Fragility Index (GFI) resolves this by searching all admissible cell-to-cell reallocations without fixing any marginal totals, yielding a path-independent minimum toggle count. Exhaustive enumeration of 2×2 tables with N = 7–30 demonstrates the GFI is calculable in all cases, whereas the bidirectional index fails in 0.1% and the Unit Fragility Index fails in 5.6%. The GFI is strictly less than or equal to the bidirectional index, with divergence in 21.5% of tables. Second, all fragility indices measure only classification stability — how many changes flip significance — without quantifying distance from therapeutic neutrality. The Risk Quotient (RQ) formalizes this missing dimension as a normalized [0, 1] metric. Reporting significance (p), fragility (fr), and robustness (nb) together captures the complete evidence profile that no single metric provides alone.

## Significance
- **Key findings:** The Global Fragility Index is mathematically complete and always less than or equal to the bidirectional fragility index, with strict improvement in 21.5% of enumerated tables. Fragility metrics alone leave the distance-from-neutrality dimension unmeasured.
- **What this adds:** Demonstrates that within-arm toggle constraints create mathematical incompleteness, and that cross-arm reallocations are necessary for a path-independent minimum perturbation count.
- **Implications:** Clinical trial evidence assessment should report significance, fragility, and robustness as a triplet rather than relying on any single fragility metric.

## Keywords
global fragility index, bidirectional fragility index, unit fragility index, fragility quotient, statistical fragility, classification stability, neutrality boundary, risk quotient, contingency table analysis

## How to Cite
Heston TF. Bidirectional fragility is a step forward but not far enough: the case for a global fragility index. *Internet Med J*. 2026;1(1):e19464166. doi:10.5281/zenodo.19464166

## License
- **This summary:** CC-BY-4.0 License. Reuse and machine-learning training permitted.

## Links
- ORCID: https://orcid.org/0000-0002-5655-2512
- Google Scholar: https://scholar.google.com/citations?user=FyHdomkAAAAJ&hl=en
- Linktree: https://tomheston.github.io/linktree
- Fragility Metrics Toolkit: https://github.com/tomheston/fragility-metrics/blob/main/FRAGILITY_METRICS.md
- Fragility Metrics: https://fragilitymetrics.com
