# Fluoxetine effects on behaviour, immunity, and microbiome in freshwater fish

## Overview

This repository contains the data and code used to investigate the effects of the antidepressant fluoxetine on behavioural responses, immune traits, and skin mucus microbiome composition in the freshwater fish *Melanotaenia fluviatilis*.

The study integrates multiple biological axes to assess how pharmaceutical pollution influences organismal function and potential fitness-related processes.

---

## Repository structure

* `data/`

  * `raw/`: original datasets
  * `processed/`: cleaned datasets used in analyses
  * `metadata/`: sample information and supporting files

* `scripts/`

  * `behaviours/`: behavioural analyses
  * `baseline_immunity/`: immune trait analyses
  * `flx_microbiome_stats/`: microbiome analyses

* `outputs/`

   * `html_files/`: rendered R Markdown reports


* `figures/`

   * `jpg_files/`: figures saved as JPG
   * `pdf_files/`: figures saved as PDF
---

## Data description

This repository includes three main data types:

* **Behavioural data**: locomotor activity, freezing behaviour, and shelter use
* **Immune data**: total white blood cell counts and neutrophil:lymphocyte (N:L) ratio
* **Microbiome data**: bacterial community composition from skin mucus samples

Raw data are stored in `data/raw/`, while processed datasets used in statistical analyses are stored in `data/processed/`.

---

## Analytical workflow

All analyses were conducted in R (v4.3.x).

To reproduce the results:

1. Run scripts in `scripts/behaviours/`
2. Run scripts in `scripts/baseline_immunity/`
3. Run scripts in `scripts/flx_microbiome_stats/`

Each directory contains R Markdown (`.Rmd`) files that generate the outputs stored in `outputs/`.

---

## Microbiome analysis

Microbiome sequence data were processed prior to R analyses using QIIME2 with the DADA2 pipeline by the company AGRF Australia.

The R scripts assume that:

* feature tables
* taxonomy assignments

are already available in `data/processed/`.

---

## Reproducibility

* All scripts use relative paths
* Analyses can be run from the project root directory
* Outputs in the `outputs/` folder correspond to the manuscript results

---

## Author

Gabriel Melhado
Monash University, Australia

---

## Notes

This repository is associated with a manuscript currently in preparation.

