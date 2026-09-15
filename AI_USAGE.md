# AI Usage — Lab 2

**Tool used:** Claude (Anthropic)

## What Claude helped with

- Helped me plan the steps needed to complete the lab given
  the rubric
- Walked me through specific steps on how to write the R code
  for loading the MIMIC-IV `admissions` and
  `diagnoses_icd` tables directly from PhysioNet using `read_csv()`.
- Walked me through specific steps on how to write
   `mutate()` code to calculate length of stay
  (`dischtime - admittime`) for each admission.
- Walked me through specific steps on how to write the
  `inner_join()` + `group_by()` + `summarize()` code to find
  average length of stay per diagnosis code, and the `filter()`/
  `arrange()` steps to narrow it to the top 10.
- Walked me through specific steps on how to write
-  the `ggplot2` code for the bar chart, including the color
  gradient styling.
- I am new to R/RStudio/Quarto, so Claude walked me step-by-step through
  using the Console, creating code chunks, and rendering the document —
  I did not know this beforehand.
- Helped draft this README.md and AI_USAGE.md file structure.
- Walked me through setting up `reticulate` for the
  mixed-language extra credit notebook, since this wasn't covered in
  lecture.

## What I did myself

- Ran every chunk and confirmed the output at each step before moving on.
- Reviewed and rewrote the interpretation section in my own words rather
  than using Claude's draft as-is.
- Set up the GitHub repository and committed/pushed the files.
