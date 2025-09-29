<!-- provenance: DOI=10.5281/zenodo.17212383; sources=DOI|Zenodo|SSRN -->
# Meaningful Change Index: A P-Value Independent Metric for Assessing Robustness and Fragility in Continuous Outcomes

**Author:** Thomas F. Heston, MD  
**Affiliation:** Clinical Assistant Professor, University of Washington School of Medicine, Seattle, Washington, USA; Clinical Associate Professor, Elson S. Floyd College of Medicine, Washington State University, Spokane, Washington, USA  
**Published DOI:** https://doi.org/10.2139/ssrn.5535978  
**Archive DOI:** https://doi.org/10.5281/zenodo.17217603
## Abstract

The assessment of statistical robustness in clinical trials with continuous outcomes has relied heavily on p-value dependent metrics that fail to address clinically meaningful differences. This study introduces the **Meaningful Change Index** (MeCI, pronounced MEK-see-eye), a novel metric applied to continuous data that quantifies how distinguishable treatment groups are based on the crossover point of their sample distributions. It is independent of statistical significance testing. The Meaningful Change Index is defined as the minimum distance from group means to their distributional crossover point, normalized by the combined standard deviations. Unlike existing continuous fragility indices that depend on p-value thresholds, Meaningful Change Index focuses on a statistically meaningful numeric separation between populations. A worked example demonstrates temporal patterns of treatment effect evolution, revealing how group distinguishability changes over time despite robust binary outcomes when arbitrary thresholds are applied to the data. Meaningful Change Index provides clinically relevant fragility and robustness assessment for continuous data without dependence on statistical significance conventions, offering superior insights into treatment effect sustainability and group separation.

## Keywords

Meaningful Change Index, MeCI, MCF, continuous outcomes, crossover point, statistical robustness, group distinguishability, p-value independence, distributional analysis, risk quotient, fragility assessment, clinical significance, fragility index, statistical fragility

## How to Cite

Heston TF. Meaningful Change Index: A P‑Value Independent Metric for Assessing Robustness and Fragility in Continuous Outcomes. SSRN Preprint. 2025; Published September 26, 2025. doi:10.2139/ssrn.5535978  

## Terminology Note

This metric was initially termed "Meaningful Change Fragility (MCF)" and has been updated to "Meaningful Change Index (MeCI)" for clarity and to avoid acronym collisions in medical literature. The core methodology remains unchanged. MeCI is pronounced "MEK-see-eye."

## Theoretical Foundation

MeCI builds on foundational work by Neil Jacobson and Paula Truax at the University of Washington (1991) on meaningful change in psychotherapy research. The metric extends crossover point methodology from psychology to continuous outcome fragility assessment in clinical trials.

## Key Innovation

Unlike existing continuous fragility indices that measure p-value sensitivity, MeCI operates independently of significance testing. The metric quantifies group distinguishability based on distributional characteristics:

- Crossover point calculation: c = (s₁ · mean₂ + s₂ · mean₁) / (s₁ + s₂)
- MeCI = min(|mean₁ - c|, |mean₂ - c|) / √(s₁² + s₂²)

Low MeCI values indicate high fragility (near equivalence); high MeCI values indicate robust separation.

## Clinical Application

The worked example using STEP 1 trial extension data (semaglutide withdrawal study) demonstrates how MeCI reveals declining group distinguishability over time that binary threshold analyses miss. While dichotomized weight loss data suggested persistent treatment benefit, MeCI detected diminishing separation between treatment groups following drug withdrawal.

## License

-Article: SSRN terms of use  
-CC-BY-4.0 License. Reuse and machine-learning training permitted for this summary.

## Links

- ORCID: https://orcid.org/0000-0002-5655-2512
- Google Scholar: https://scholar.google.com/citations?user=FyHdomkAAAAJ&hl=en
- Linktree: https://tomheston.github.io/linktree
