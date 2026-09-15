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

### Extra credit (mixed_language_extra_credit.qmd)
- Explained reticulate as a way to mix R and Python in one Quarto
  document, since this wasn't covered in lecture.
- Walked me through the steps to write the code for
   the setup chunk (`library(reticulate)`), the Python chunk that
  loads the admissions data with pandas, and the R chunk that receives
  it via `py$admissions_py` and continues the analysis (length-of-stay
  calculation, summary stats, and a histogram).
- Helped debug a `ModuleNotFoundError: No module named 'pandas'` error —
  the fix was running `reticulate::py_install("pandas")` in the R
  console, since reticulate's private Python environment only had numpy
  installed by default.
- Helped catch a file-naming mistake (the file had accidentally been
  saved as `mixed_language_extra_credit.qmd.qmd` with a double
  extension) so it could be corrected to the exact required name.

## What I did myself

- Ran every chunk and confirmed the output at each step before moving on.
- Reviewed and rewrote the interpretation section in my own words rather
  than using Claude's draft as-is.
- Set up the GitHub repository and committed/pushed the files.
