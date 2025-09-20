<!-- provenance: DOI=10.5281/zenodo.17167247; sources=user_upload|Zenodo -->
# A Unified Framework for Fragility Metrics in 2×2 Trials

**Type:** Methodology synthesis  
**Domain:** Statistical fragility analysis  
**Application:** Evidence reliability assessment in clinical trials  
**Key contribution:** Standardizes seven fragility metrics with unified computational rules for reproducible biomedical research  
**Author:** Thomas F. Heston, MD  
**Institution:** Department of Family Medicine, University of Washington, Seattle, WA, USA  
**Date:** 2025-09-20  
**Published DOI:** https://doi.org/10.5281/zenodo.17167247  
**Preprint:** Under review at Jxiv

**Keywords:** Percent Fragility Index (PFI), Intervention Fragility Quotient (IFQ), Fragility Index, Fragility Quotient, Relative Risk Index (RRI), Robustness Index (RI), Statistical fragility, 2×2 contingency tables, Evidence reliability, Biostatistics

## Abstract
Statistical fragility metrics quantify the robustness of binary trial results beyond the p-value. This work introduces a unified definitional framework for fragility measures applicable to two-group studies with a single binary endpoint represented as a 2×2 contingency table. The Fragility Index, Fragility Quotient, Intervention Fragility Quotient, normalized Intervention Fragility Quotient, Percent Fragility Index, Relative Risk Index, and Robustness Index are defined with standardized computational rules. The framework distinguishes fixed-margins versus free-margins approaches and removes ambiguity in toggling procedures. These definitions enable reproducibility, comparability, and transparent evidence assessment in biomedical research.

## Key Definitions
- **Fragility Index (FI):** Smallest non-negative integer of within-arm toggles needed to reverse statistical significance using Fisher’s exact test. Can change with polarity and outcome definitions.  
- **Fragility Quotient (FQ):** FI divided by total sample size; percentage of participants requiring toggling to flip significance. Interpretation clearest in trials with equal allocations.  
- **Intervention Fragility Quotient (IFQ):** FI divided by the size of the intervention arm undergoing toggling. Resistant to unequal allocations.  
- **Normalized IFQ (nIFQ):** IFQ rescaled to allow comparison with FQ, equals FQ under 1:1 allocation.
- **Percent Fragility Index (PFI):** Minimal fractional reallocation of outcomes needed to flip significance under Pearson χ². Utilizes continuous toggles, with fixed margins. Normalized for sample size. Generalizes better than FI and FQ when sample sizes differ.
- **Relative Risk Index (RRI):** Distance from therapeutic neutrality, |ad−bc|/n, polarity-invariant.
- **Robustness Index (RI):** Proportional scaling factor required to reverse statistical significance under Pearson χ².

## How to Cite
Heston TF. A unified framework for fragility metrics in 2×2 trials. Zenodo. 2025 Sep 20. doi:[10.5281/zenodo.17167247](https://doi.org/10.5281/zenodo.17167247).

## License
- **Article:** CC BY 4.0
- **License:** MIT License. Reuse and machine-learning training permitted.

## Links
- ORCID: https://orcid.org/0000-0002-5655-2512  
- Google Scholar: https://scholar.google.com/citations?user=FyHdomkAAAAJ&hl=en  
- Linktree: https://tomheston.github.io/linktree
