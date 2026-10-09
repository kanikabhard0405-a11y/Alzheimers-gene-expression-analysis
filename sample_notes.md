# Research Notes: Alzheimer's Gene Expression

## Dataset

* **AD dataset:** GSE48350
* **Normal control dataset:** GSE11882
* **Organism:** Homo sapiens

## Study Design

* AD cases are labeled `AD`.
* Normal controls are labeled `indiv`.
* Controls include young and aged individuals.
* Tissue consists of postmortem brain samples collected from ADRC brain banks.
* AD cases and controls were processed simultaneously.

## Sample Observed

* **Sample title:** superior frontal gyrus_male_94_AD_90
* **Brain region:** Superior frontal gyrus
* **Sex:** Male
* **Age:** 94 years
* **Braak stage:** IV
* **APOE genotype:** 3,3

## Planned Analysis

Compare gene expression between Alzheimer's disease and normal control samples from the same brain region, after checking sample metadata and data compatibility.

## Limitations and Checks

* Confirm the disease/control assignment for each sample.
* Check age and brain-region differences.
* Verify that expression measurements from the two datasets are compatible before combining them.
* No gene-expression comparisons have been performed yet.

## Control Sample Identified

* **Dataset:** GSE11882
* **Sample title:** SuperiorFrontalGyrus_male_40yrs_indiv68
* **Group:** Normal control, based on the study's `indiv` label
* **Brain region:** Superior frontal gyrus
* **Sex:** Male
* **Age:** 40 years

### Preliminary Comparison

The control and AD samples match by brain region and sex, but their ages differ substantially (40 versus 94 years). This age difference is a potential confounding factor. This single sample pair is for learning metadata interpretation only; it is not sufficient for a reliable gene-expression comparison.

## Additional Control Sample

* **Dataset:** GSE11882
* **Sample title:** SuperiorFrontalGyrus_male_80yrs_indiv15
* **Group:** Normal control (`indiv`)
* **Brain region:** Superior frontal gyrus
* **Sex:** Male
* **Age:** 80 years

### Preliminary Matching Decision

This control is a closer match to the 94-year-old male AD sample than the previously recorded 40-year-old control. Brain region and sex match, but a 14-year age difference remains.

A second potential control is `SuperiorFrontalGyrus_female_91yrs_indiv94` (91-year-old female). Although its age is closer to the AD sample, sex differs.

**Important limitation:** These are candidate samples for learning metadata interpretation, not a validated analysis cohort. A reliable comparison requires multiple samples, confirmation of sample annotations, and compatible expression data.
