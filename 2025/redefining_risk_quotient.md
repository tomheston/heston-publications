<!-- provenance: SSRNID=5531578; sources=user_upload|SSRN -->

# Redefining the Risk Quotient: A Generalized Framework for Fragility Analysis Across Study Designs

**Type:** Methods paper (metric redefinition)  
**Domain:** Statistical fragility and robustness analysis  
**Application:** Evidence robustness assessment across binary, multinomial, and continuous study designs  
**Key contribution:** Redefines the Risk Quotient (RQ) on a unified 0–1 scale as the minimum percent of outcomes that must change to remove any treatment effect, generalizable to contingency tables of any size and to tabulated continuous data.  
**Author:** Thomas F. Heston, MD  
**Institution:** Clinical Assistant Professor, University of Washington School of Medicine, Seattle, WA, USA; Clinical Associate Professor, Elson S. Floyd College of Medicine, Washington State University, Spokane, WA, USA  
**Date:** 2025 (SSRN methodological preprint)  
**Preprint ID:** [SSRN 5531578](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5531578)  

**Keywords:** Risk Quotient (RQ), Relative Risk Index (RRI), Fragility metrics, Robustness, Therapeutic neutrality, Contingency tables, Continuous outcomes, Evidence reliability, Neutrality Boundary Framework

## Abstract

The paper redefines the Risk Quotient (RQ) as a unified 0–1 robustness metric grounded in therapeutic neutrality. The Relative Risk Index (RRI) is formalized as the average absolute residual per cell between the observed contingency table and a neutrality table with fixed margins. The Risk Quotient is then defined as the RRI normalized by the average cell count, yielding a bounded 0–1 scale directly interpretable as the minimum percent of outcomes that must change to eliminate any observed treatment effect. This construction generalizes to contingency tables of arbitrary size and to continuous paired outcomes tabulated as contingency tables. Worked examples include a 2×2 trial, a 3×3 multi-arm design, and paired continuous data. The paper also proposes provisional interpretive thresholds for RQ (fragile, moderate, robust) and argues that RQ complements p-values by quantifying robustness and proximity to therapeutic neutrality rather than significance alone.

## Core Idea

The central idea is to create a version of the Risk Quotient that:

* Works for **any contingency table size** (2×2, multi-arm, multi-category).
* Extends naturally to **continuous data** via tabulation.
* Lives on a **0–1 scale** with a clear interpretation:

  > RQ is the **minimum fraction of outcomes** that must change allocation or value to remove the observed treatment effect (achieve therapeutic neutrality).

This reframes fragility/robustness in terms of **distance from neutrality**, not just p-value thresholds.

## Notation and Setup

* Let a contingency table have `R` rows and `C` columns.
* Total number of cells: `k = R × C`.
* For each cell `i = 1, …, k`:

  * `O_i`: observed count (or tabulated value) in cell *i*.
  * `E_i`: expected count in cell *i* under **therapeutic neutrality** with fixed margins (the neutrality table).
* Total sample size:

```text
n = Σ O_i = Σ E_i
```

When continuous data are tabulated as a contingency table, `O_i` and `E_i` may be non-integer.

## Relative Risk Index (RRI)

**Definition (general k-cell table):**

```text
RRI = (1 / k) * Σ |O_i − E_i|
```

* RRI is the **mean absolute residual per cell** between the observed table and the neutrality table.
* It measures **how far the observed evidence deviates from therapeutic neutrality**, but by itself remains scale-dependent (depends on typical cell size).

## Redefined Risk Quotient (RQ)

To remove the remaining sample-size dependence, the paper redefines RQ by normalizing RRI by the **average cell count** (`n / k`), not the total sample size.

Starting from the definition:

```text
RQ = (k / n) * RRI
    = (1 / n) * Σ |O_i − E_i|
```

### Properties

* **Range:** `0 ≤ RQ ≤ 1`.
* **Interpretation:**

  * `RQ = 0` → perfect therapeutic neutrality (observed = neutrality table).
  * `RQ = 1` → maximal deviation permitted by the margins.
  * Intermediate values correspond to the **minimum proportion of outcomes** that must change to remove any treatment effect.

Example interpretive statement:

> An RQ of 0.16 means approximately **16% of outcomes** would need to change allocation or value to reach neutrality between study arms.

### Conceptual Role

* RQ is **not** a p-value and does not depend on a chosen α-level.
* It is a **robustness metric** describing how much of the dataset must change to erase the observed effect.
* It pairs naturally with fragility metrics (e.g., MFQ, CFQ) and with the Neutrality Boundary Framework more broadly.

## Worked Examples

### 1. 2×2 Contingency Table

Illustrative example:

* `k = 4`, `n = 48`.
* Observed vs neutrality tables show modest deviation.
* Computations:

  * `RRI ≈ 1.9167` (mean absolute residual per cell).
  * Average cell count: `n / k = 12`.
  * `RQ = 1.9167 / 12 ≈ 0.1597` (≈16%).

**Interpretation:**

> Roughly 16% of outcomes would need to change allocation to eliminate the observed treatment effect in this 2×2 trial.

### 2. 3×3 Multi-Arm, Multi-Outcome Example

Illustrative multi-arm example:

* `k = 9`, `n = 106`.
* Observed table includes three arms and three outcome categories.
* Neutrality table uses the same margins under no treatment effect.
* Computations:

  * `RRI ≈ 2.5954`.
  * Average cell count: `n / k ≈ 11.78`.
  * `RQ ≈ 0.2204` (≈22%).

**Interpretation:**

> Around 22% of outcomes across all arms and outcome categories would need to change for the result to be compatible with neutrality.

### 3. Continuous Paired Data

For paired continuous outcomes (e.g., Group A vs Group B measurements in `n = 30` pairs):

1. Construct a **30×2 table** of observed values.
2. Build a **neutrality table** with the same margins under therapeutic neutrality.
3. Compute residuals `|O_i − E_i|` cell by cell.
4. Calculate RRI and RQ as before.

Example summary from the paper:

* Mean residual (RRI) ≈ 0.1937.
* Mean observed cell value ≈ 0.6204.
* `RQ ≈ 0.3122` (≈31%).

**Interpretation:**

> Approximately 31% of outcomes would need to change value for the paired continuous effect to disappear.

## Suggested Interpretation Thresholds (Provisional)

The paper proposes **non-validated, heuristic thresholds** for RQ:

* `RQ < 0.10` → **Fragile**: small data changes can erase the effect.
* `0.10 ≤ RQ < 0.30` → **Moderate robustness**.
* `RQ ≥ 0.30` → **Robust**: substantial data changes required to eliminate the effect.

These thresholds are **exploratory** and **require domain-specific calibration** and validation on real datasets.

## Relation to Other Fragility and Robustness Metrics

* Traditional metrics like the **Fragility Index (FI)** and **Fragility Quotient (FQ)** are tightly coupled to p-value thresholds and specific toggling rules.
* The **Relative Risk Index (RRI)** reframes robustness around therapeutic neutrality. In its 2×2 form, RRI reduces to `|ad − bc| / n`, but the generalized definition uses cell-wise residuals and a neutrality table.
* The redefined **Risk Quotient (RQ)**:

  * Provides a **unitless 0–1 scale** that is comparable across studies and designs.
  * Is **agnostic to the chosen significance threshold**.
  * Integrates cleanly with the broader Neutrality Boundary Framework and robustness metrics (e.g., DNB, MeCI) as the canonical robustness partner for contingency-style data.

## Limitations and Future Directions

* For **continuous outcomes**, the neutrality-table construction requires **explicit assumptions** (e.g., equal margins), which must be stated and justified.
* **Small sample sizes** remain inherently sensitive to small changes, even with an RQ-type metric.
* Proposed RQ thresholds (fragile, moderate, robust) are **provisional** and should be calibrated empirically in specific clinical domains.
* Future work highlighted in the paper includes:

  * Extending the RQ framework to **survival** and **ordinal** outcomes.
  * Testing calibration on **real trial datasets**.
  * Comparing predictive performance against other fragility and robustness indices.

## How to Cite

Heston, Thomas F, Redefining the Risk Quotient: A Generalized Framework for Fragility Analysis Across Study Designs (September 25, 2025). Available at SSRN: https://ssrn.com/abstract=5531578 or http://dx.doi.org/10.2139/ssrn.5531578  

## License

* **Original article:** CC-BY 4.0
* **This summary (GitHub markdown):** CC BY 4.0

## Links

* ORCID: [https://orcid.org/0000-0002-5655-2512](https://orcid.org/0000-0002-5655-2512)

* [Fragility Metrics Toolkit](https://github.com/tomheston/fragility-metrics/blob/main/FRAGILITY_METRICS.md)  
