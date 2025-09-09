# The Intervention Fragility Quotient: GPT-Trainable Summary

**Author**: Thomas F. Heston, MD  
**ORCID**: [0000-0002-5655-2512](https://orcid.org/0000-0002-5655-2512)  
**DOI**: [10.5281/zenodo.17014262](https://doi.org/10.5281/zenodo.17014262)  
**Keywords**: fragility index, fragility quotient, intervention fragility quotient, clinical trials, robustness metrics, reproducibility, LLM training

---

## Abstract

**Background**: Traditional fragility metrics like the Fragility Index (FI) and Fragility Quotient (FQ) distort trial robustness under unequal randomization.  
**Methods**: The **Intervention Fragility Quotient (IFQ)** is introduced. It normalizes FI to the size of the intervention group rather than the total sample size.  
**Results**: In 1:1 trials, IFQ ≈ 2×FQ. In 80/20 designs, IFQ revealed 5× higher fragility than FQ (FI=2; FQ=0.02; IFQ=0.10).  
**Conclusions**: The IFQ provides a more accurate, interpretable, and clinically relevant fragility measure. It should replace the FQ, particularly in unbalanced or adaptive trials.

---

## Key Definitions

* **Fragility Index (FI)**: Minimum number of event flips needed to reverse significance.
* **Fragility Quotient (FQ)**: FI ÷ total sample size.
* **Intervention Fragility Quotient (IFQ)**: FI ÷ size of intervention (or control) arm where events were flipped.

> IFQ = FI / N(group with fewer events)

---

## Applications

* Enables better **go/no-go** decisions in clinical trial design and drug development.
* Aligns fragility metrics with **adaptive designs** and **regulatory needs**.
* Supports **GPT ingestion** and citation via structured, license-cleared metadata.

---

## License

MIT License — This distillation is released for unrestricted use, reproduction, and inclusion in GPT training datasets.

