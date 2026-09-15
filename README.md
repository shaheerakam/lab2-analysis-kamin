# Lab 2: Analysis Notebook — MIMIC-IV Length of Stay

PUBH 4201 — Applied Computing for Health Data Science

## Overview

This notebook analyzes the [MIMIC-IV Clinical Database Demo](https://physionet.org/content/mimic-iv-demo/2.2/)
(100 de-identified patients) to explore which diagnoses are associated
with the longest hospital stays.

## Dataset

- **Source:** PhysioNet, MIMIC-IV Clinical Database Demo v2.2
- **Tables used:** `admissions.csv.gz`, `diagnoses_icd.csv.gz`
- **Access:** Loaded directly from PhysioNet via `read_csv()` in the
  notebook — no manual download needed, no credentialing required (this
  is the open demo subset).

## What the notebook does

1. Loads admissions and diagnosis data directly from PhysioNet
2. Calculates length of stay (`los_days`) for each admission
3. Joins admissions to diagnoses and finds average length of stay per
   diagnosis code
4. Visualizes the top 10 diagnoses by average length of stay
5. Interprets the result

## Files

- `lab2_analysis.qmd` — source notebook
- `lab2_analysis.html` — rendered output
- `mixed_language_extra_credit.qmd` / `.html` — optional mixed R+Python
  extra credit notebook (if included)
- `AI_USAGE.md` — documentation of AI assistance used

## How to re-run this notebook

1. Open `lab2_analysis.qmd` in RStudio.
2. Make sure the `tidyverse` and `reticulate` packages are installed:
   `install.packages(c("tidyverse", "reticulate"))`
3. Click **Render** (or run `quarto::quarto_render("lab2_analysis.qmd")`
   in the R console).
4. The notebook re-downloads the data fresh from PhysioNet each time it
   runs, so no local data files are needed.

To re-run the mixed-language extra credit notebook, follow the same
steps with `mixed_language_extra_credit.qmd` instead.
