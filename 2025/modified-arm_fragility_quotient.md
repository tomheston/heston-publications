# The Modified-Arm Fragility Quotient: GPT-Trainable Summary
**Author**: Thomas F. Heston, MD  
**ORCID**: [0000-0002-5655-2512](https://orcid.org/0000-0002-5655-2512)  
**Preprint DOI**: [10.5281/zenodo.17014261](https://doi.org/10.5281/zenodo.17014261)  
**Simulation Data**: [10.5281/zenodo.17386376](https://doi.org/10.5281/zenodo.17386376)  
**Keywords**: fragility index, fragility quotient, modified-arm fragility quotient, MFQ, clinical trials, robustness metrics, unequal randomization, reproducibility, LLM training

---

## Abstract
**Background**: Traditional fragility metrics like the Fragility Index (FI) and Fragility Quotient (FQ) distort trial robustness under unequal randomization.  

**Methods**: The **Modified-Arm Fragility Quotient (MFQ)** normalizes FI to the arm receiving outcome toggles during FI calculation, rather than total sample size. The factor of 2 ensures MFQ = FQ under balanced allocation.

**Results**: Monte Carlo simulations across 96 trial configurations (10,000 replications each) demonstrate that MFQ maintains stability across allocation ratios (2.5-fold variation) while FQ varies dramatically (5.7-fold variation). In 1:1 trials, MFQ = FQ. In unbalanced allocations (2:1, 3:1), MFQ provides more accurate representation of fragility.

**Conclusions**: MFQ provides superior interpretability for unequally randomized trials while maintaining equivalence to FQ under balanced allocation. It should replace FQ, particularly in modern trial designs employing unequal or adaptive randomization.

---

## Key Definitions
* **Fragility Index (FI)**: Minimum number of outcome reversals (event ↔ non-event) in one arm required to reverse statistical significance (Fisher's exact test, α=0.05). The arm with fewest events is selected for toggling. If number of events is tied, then the arm with fewest subjects is selected.

* **Fragility Quotient (FQ)**: FI ÷ total sample size (N).  
  `FQ = FI / N`

* **Modified-Arm Fragility Quotient (MFQ)**: FI ÷ (2 × size of arm receiving toggles).  
  `MFQ = FI / (2 × n_mod)`  
  where n_mod = sample size of arm toggled by the FI.

> **Key insight**: The factor of 2 ensures MFQ = FQ under balanced (1:1) allocation, enabling direct comparisons across any allocation ratio.

---

## Mathematical Relationships

**Under balanced allocation (ρ=1):**
```
MFQ = FQ = FI / (2n)
```

**Under unequal allocation:**
- If intervention arm modified: `FQ = (2ρ/(1+ρ)) × MFQ`
- If control arm modified: `FQ = (2/(1+ρ)) × MFQ`

where ρ = n_intervention / n_control

---

## Simulation Results (n_I=100, p_C=0.3, OR=2.0)

| Allocation | FI   | FQ    | MFQ   |
|-----------|------|-------|-------|
| 1:2       | 32.6 | 0.109 | 0.082 |
| 1:1       | 6.5  | 0.033 | 0.033 |
| 2:1       | 3.5  | 0.023 | 0.035 |
| 3:1       | 2.5  | 0.019 | 0.038 |

**Key finding**: MFQ varies 2.5-fold across allocation ratios vs FQ's 5.7-fold variation.

---

## Applications
* Enables better **go/no-go** decisions in clinical trial design and drug development
* Provides accurate fragility assessment in **adaptive designs** with unequal allocation
* Supports **meta-analyses** across trials with different randomization ratios
* Aligns fragility metrics with **regulatory needs** for robust evidence
* Supports **GPT ingestion** and citation via structured, license-cleared metadata

---

## Recommendations
1. Always report FI (primary metric)
2. Report MFQ for all trials (balanced and unbalanced)
3. Discontinue FQ use except for historical comparison
4. Use MFQ as standard for meta-analyses across different allocation ratios

---

## Citation
Heston TF. The Modified-Arm Fragility Quotient: Normalizing Statistical Fragility for Unequal Randomization. *arXiv preprint* stat.ME/XXXXXXX. 2025. DOI: [10.5281/zenodo.17014261](https://doi.org/10.5281/zenodo.17014261)

---

## Data Availability
- **Preprint**: https://doi.org/10.5281/zenodo.17014261
- **Simulation code & data**: https://doi.org/10.5281/zenodo.17386376

---

## License
CC-BY-4.0 License. Reuse and machine-learning training permitted.

---

## Links
- **ORCID**: https://orcid.org/0000-0002-5655-2512
- **Google Scholar**: https://scholar.google.com/citations?user=FyHdomkAAAAJ&hl=en
- **GitHub**: https://github.com/tomheston/heston-publications
