Fluoxetine effects on behaviour, immunity, and microbiome in freshwater fish
Overview

This repository contains all data and code used to analyse the effects of the antidepressant fluoxetine on behavioural responses, immune traits, and skin mucus microbiome composition in freshwater fish (Melanotaenia fluviatilis).

The project integrates multiple biological axes to assess how pharmaceutical pollution influences organismal function and potential fitness-related traits.

Repository structure
.
├── data/              # Metadata and sample information
│
├── scripts/
│   ├── behaviour/     # Behavioural analyses (GLMMs, plotting)
│   ├── immunity/      # Immune trait analyses (WBC, N:L ratio)
│   └── vsearch/       # Microbiome analyses (phyloseq, diversity)
│
├── outputs/
│   └── html_reports/     # Rendered R Markdown reports
│
└── README.md

Data description
Behavioural data: locomotor activity, freezing behaviour, and shelter use
Immune data: total white blood cell counts and neutrophil (N) ratio
Microbiome data: skin mucus bacterial community composition derived from 16S rRNA sequencing

Raw data are stored in data/raw/. Processed datasets used for modelling are stored in data/processed/.

Analytical workflow

Analyses were conducted in R (version 4.3.x). Statistical models were primarily fitted using the glmmTMB framework, and microbiome analyses were performed using phyloseq.

To reproduce the analyses:

Run behavioural analyses:
scripts/behaviour/
Run immune analyses:
scripts/immunity/
Run microbiome analyses:
scripts/vsearch/

Each folder contains R Markdown (.Rmd) files that generate the outputs stored in outputs/.

Reproducibility

All scripts use relative paths and can be run from the project root directory.

To fully reproduce results:

Ensure required R packages are installed
Follow the workflow order described above
Use the processed datasets provided

Citation

If you use this repository or associated data, please cite the corresponding manuscript (to be added upon publication).

Author

Gabriel Melhado
School of Biological Sciences
Monash University, Australia
