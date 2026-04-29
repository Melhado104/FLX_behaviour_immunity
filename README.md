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

  * `01_behaviour/`: behavioural analyses
  * `02_immunity/`: immune trait analyses
  * `03_microbiome/`: microbiome analyses

* `outputs/`

  * `figures/`: figures used in the manuscript
  * `tables/`: statistical outputs
  * `html_reports/`: rendered R Markdown reports

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

1. Run scripts in `scripts/01_behaviour/`
2. Run scripts in `scripts/02_immunity/`
3. Run scripts in `scripts/03_microbiome/`

Each directory contains R Markdown (`.Rmd`) files that generate the outputs stored in `outputs/`.

---

## Microbiome analysis

Microbiome sequence data were processed prior to R analyses using QIIME2 with the DADA2 pipeline.

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

