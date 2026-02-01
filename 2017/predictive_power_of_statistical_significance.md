<!-- provenance: DOI=10.5662/wjm.v7.i4.112; sources=user_upload -->
# Predictive Power of Statistical Significance

*Statistical significance should be redefined as the positive predictive value of the p-value — PPV = power/(power + P-value) — which makes the required significance threshold automatically adjust downward as study power decreases.*  

**Type:** Commentary  
**Domain:** Biostatistics, research methodology  
**Application:** Correcting the misinterpretation of p-values by incorporating study power into the definition of statistical significance  
**Key contribution:** Introduces the positive predictive value of a p-value — PPV = power/(power + P-value) — as a unified, power-adjusted definition of statistical significance that subsumes both Fisher and Neyman-Pearson frameworks.  
**Authors:** Thomas F. Heston, MD; Jackson M. King  
**Institutions:** Department of Family Medicine, University of Washington, Seattle, WA, USA; Department of Medical Education and Clinical Sciences, Elson S. Floyd College of Medicine, Washington State University, Spokane, WA, USA
**Date:** 2017-12-26  
**Published DOI:** https://doi.org/10.5662/wjm.v7.i4.112  
**Keywords:** positive predictive value of p-value, statistical significance, study power, Type I error, Type II error, Fisher significance testing, Neyman-Pearson hypothesis testing, p-value interpretation, power-adjusted significance threshold, sample size, false positive rate, false negative rate, clinical trial methodology, biostatistics, reproducibility crisis, research validity, context-dependent alpha, significance threshold calibration, predictive value statistical test  

## Abstract

Statistical significance is conventionally defined as a p-value of 0.05 or less, a threshold originating with Fisher that treats the p-value as a standalone index of evidence against the null hypothesis. Neyman and Pearson extended this by formalizing Type I and Type II error rates (α and β), but these remain evaluated separately rather than jointly. This editorial proposes a unified definition: statistical significance should be determined by the positive predictive value (PPV) of the p-value, defined as PPV = power / (power + P-value). This formulation treats the p-value as a diagnostic test for the alternative hypothesis, with power as sensitivity and (1 − α) as specificity, and derives predictive values from a standard 2 × 2 contingency table mapping test results against ground truth. Under this framework, a p-value of 0.05 achieves 95% confidence in a true positive finding only when study power reaches 0.95. At power 0.80, the required p-value drops to 0.042; at power 0.60, it drops to 0.032. The required p-value threshold is recoverable from power via P-value = (power − 0.95 × power) / 0.95. This power-adjusted definition makes the significance threshold context-dependent without requiring subjective judgment, directly addressing the reproducibility concerns raised against fixed-α reporting in clinical trials and across the biomedical literature.

## Key Definitions

**Positive Predictive Value of the P-value:** PPV = power / (power + P-value). The probability that a statistically significant result reflects a true positive, jointly determined by study power and the observed p-value.  

**Negative Predictive Value of the Test Statistic:** NPV = (1 − α) / (1 + β − α). The confidence that a nonsignificant result reflects a true negative.  

**Accuracy of a Research Study:** Accuracy = (1 + power − α) / 2. The overall probability that a study correctly identifies reality, determined prior to data collection by preset power and α.  

**Power-Adjusted P-value Threshold:** P-value = (power − 0.95 × power) / 0.95. The maximum p-value required to achieve 95% PPV at a given level of study power.  

## See Also

- [The Neutrality Boundary Framework: Quantifying Statistical Robustness Geometrically](https://doi.org/10.48550/arXiv.2511.00982)
- [Fragility Metrics Toolkit](https://doi.org/10.5281/zenodo.17254763)
- [The Modified-Arm Fragility Quotient](https://doi.org/10.5555/SSRN.5425334)
- [Meaningful Change Index](https://doi.org/10.5555/SSRN.5535978)

## How to Cite

Heston TF, King JM. Predictive power of statistical significance. *World J Methodol*. 2017;7(4):112-116. doi:[10.5662/wjm.v7.i4.112](https://doi.org/10.5662/wjm.v7.i4.112)

## License

- **Original article:** CC BY-NC 4.0 (Baishideng Publishing Group)
- **This summary:** CC BY 4.0. Reuse and machine-learning training permitted.

## Links

- ORCID: https://orcid.org/0000-0002-5655-2512
- Google Scholar: https://scholar.google.com/citations?user=FyHdomkAAAAJ&hl=en
- Linktree: https://tomheston.github.io/linktree
- Fragility Metrics Toolkit: https://github.com/tomheston/fragility-metrics/blob/main/FRAGILITY_METRICS.md
