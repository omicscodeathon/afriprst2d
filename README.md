# afriprst2d
A Reproducible Polygenic Risk Score Pipeline for Type 2 Diabetes in African Populations

## Overview
The aim of this project is to build a reproducible polygenic risk score pipeline for detecting Type 2 Diabetes amongst African population. Due to the limited availability of African datasets, genetic diversity and different patterns of variation for Type 2 Diabetes, this reproducible pipeline aims to bridge the gap created by PRS models trained on European data.

## Status
- Literature review: 31 articles collected, synthesis in progress
- Data: 2 datasets identified, access pending.
- Pipeline development: [started]

The workflow covers GWAS quality control, SNP harmonization, P-value thresholding, LD clumping, PRS weight generation, and—once independent target data become available—PRS calculation and validation.

## Workflow

**T2D GWAS Summary Statistics → GWAS QC → SNP Harmonization → African LD Reference → LD Clumping → P-value Thresholding → PRS Weights → Target Genotype Data → PRS Calculation → Standardization → Phenotype Data → Validation**

## Data Used For the Pipeline

### 1. T2D GWAS Summary Statistics

**Source:** MVP African-ancestry T2D GWAS

The GWAS summary statistics contain variant-level association information including:

* SNP identifier
* Chromosome and position
* Effect and non-effect alleles
* Effect allele frequency
* Beta
* Standard error
* P-value
* Sample size

The summary statistics are used as the **discovery GWAS** for the PRS pipeline.


### 2. African LD Reference Panel

**Reference:** 1000 Genomes Phase 3 African-ancestry samples

The African reference panel is used to estimate linkage disequilibrium (LD) between variants during LD clumping.

Current reference files:

```text
AFR_only.pgen
AFR_only.pvar
AFR_only.psam
```

The reference contains **661 individuals from African populations** represented in the 1000 Genomes Phase 3 dataset.

## Current Pipeline Status

The discovery and PRS-construction stages are being developed using the available GWAS summary statistics and African LD reference panel.

### Completed / In progress

* [x] T2D GWAS summary statistics obtained
* [x] GWAS quality control
* [x] SNP harmonization
* [x] Candidate SNP generation across multiple P-value thresholds
* [ ] LD clumping
* [ ] PRS weight generation
* [ ] PRS calculation in an independent target cohort
* [ ] PRS standardization
* [ ] Phenotype-based validation

## Target Genotype and Phenotype Data

**Independent target genotype and phenotype data are not currently available.**

Therefore, the final stages of the workflow cannot yet be performed.

Specifically, we currently do **not** have an independent African target dataset containing:

```text
Genotype data
+
T2D phenotype / relevant clinical phenotype
```

These data are required to calculate individual-level PRS and evaluate predictive performance.

Once an appropriate independent African genotype–phenotype dataset is obtained, the workflow will proceed to:

1. Apply the derived PRS weights to the target genotype data.
2. Calculate individual-level PRS.
3. Standardize the PRS.
4. Merge PRS with target phenotype and covariate data.
5. Perform statistical validation.
6. Evaluate model performance using measures such as logistic regression and ROC/AUC.

## P-value Thresholds

The current workflow evaluates multiple P-value thresholds:

```text
5 × 10⁻⁸
1 × 10⁻⁵
1 × 10⁻⁴
1 × 10⁻³
1 × 10⁻²
5 × 10⁻²
```

This allows the resulting PRS models to be evaluated across different levels of GWAS variant inclusion once an independent target cohort becomes available.

## Reproducibility

The workflow is implemented using reproducible computational steps and is organized so that intermediate outputs can be retained and reused rather than regenerated unnecessarily.

Primary tools include:

* **Python**
* **pandas**
* **PLINK 2.0**
* **1000 Genomes Phase 3**

## Repository Structure

```text
t2d-prs/
│
├── README.md
│
├── workflow/
│   └── T2D_PRS_workflow/
│
├── gwas/
│   └── GWAS summary statistics
│
├── reference/
│   └── African LD reference panel
│
├── results/
│   ├── gwas_qc/
│   ├── harmonized/
│   ├── candidate_snps/
│   ├── ld_clumping/
│   └── weights/
│
└── notebooks/
    └── analysis notebooks
```

## Important Data Status

> **The current project has discovery GWAS summary statistics and an African LD reference panel, but does not yet have independent target genotype and phenotype data.**

Consequently, **a validated individual-level T2D PRS has not yet been produced**. The target-cohort calculation and predictive validation stages will be completed when suitable independent African genotype–phenotype data become available.

### Project Workflow

**[Open the complete T2D PRS Workflow →](./figures/Workflow 1.png)**

