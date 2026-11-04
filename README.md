# Cumulative Study Guide: Business Statistics with R

A comprehensive, cumulative study guide and computational reference for applied 
business statistics. This repository combines textbook theory, mathematical
formulas, and practical R implementations covering concepts from:

---

## Overview

This repository provides reproducible study materials designed to reinforce core
statistical foundations and their application in R. Each module includes:
- **Conceptual Summaries:** Clear definitions, core business use cases, and
  statistical terminology.
- **Mathematical Formulations:** LaTeX-rendered formulas for descriptive and 
  inferential statistics.
- **R Code Implementations:** Reproducible scripts for data classification,
  descriptive tables, frequency distributions, and visual diagnostics
  (histograms, polygons, ogives, Pareto charts, and scatter plots).

---

## Repository Structure

```text
CumulativeStudyGuide/
├── README.md               # Repository documentation and curriculum overview
├── Week1.Rmd               # Source R Markdown document for Week 1 (Chapters 1 & 2)
├── Week1.html              # Rendered HTML study guide with floating TOC
├── Week1_files/            # Supporting assets and dependencies for HTML output
├── Week7.Rmd               # Source R Markdown document for Week 7 (Chapter 10)
└── Week7.html              # Rendered HTML study guide with floating TOC
```

---

## Course & Topic Outline

| Module | Textbook Chapters | Key Topics | R Implementations |
| :--- | :--- | :--- | :--- |
| **Week 1** | **Ch. 1:** Intro to Statistics<br>**Ch. 2:** Charts & Graphs | • Populations vs. Samples<br>• Levels of Measurement (Nominal, Ordinal, Interval, Ratio)<br>• Frequency distributions, class marks, relative & cumulative frequency<br>• Graphical displays & Pareto analysis<br>• Ethical data presentation | • `factor()` / ordered factors<br>• Frequency tables (`cut()`, `table()`)<br>• `hist()`, frequency polygon, ogive<br>• `stripchart()` dot plots & `stem()`<br>• `barplot()`, `pie()`, & Pareto charts<br>• Two-variable `plot()` with `lm()` regression line |
| **Week 7** | **Ch. 10:** Inferences About Two Populations | • Test selection framework<br>• Difference in two means ($\sigma$ known vs. unknown)<br>• Pooled vs. Welch's unequal-variance $t$-tests<br>• Matched-pairs / related populations<br>• Two-proportion $z$-tests & pooling<br>• Two-variance $F$-tests<br>• Ethical comparative analysis<br>• **44 Exam & Study Questions with Full Solutions** | • Custom `two_sample_z_test()`<br>• `t.test(..., var.equal = TRUE)`<br>• `t.test(..., var.equal = FALSE)`<br>• `t.test(..., paired = TRUE)`<br>• `prop.test(..., correct = FALSE)`<br>• `var.test()` |

*(Additional weekly modules will be added as the study guide expands.)*

---

## Prerequisites & Setup

### R Environment
- **R version:** $\ge$ 4.0.0
- **Recommended IDE:** [Positron](https://github.com/posit-dev/positron) or RStudio

### Required R Packages
Install the necessary visualization and publishing packages from CRAN:

```r
install.packages(c("rmarkdown", "knitr", "ggplot2", "gridExtra"))
```

---

## Rendering the Study Guides

Each study guide is authored in R Markdown (`.Rmd`) and configured to compile into a standalone HTML report with a floating table of contents.

To render via the R console:

```r
# Render Week 1
rmarkdown::render("Week1.Rmd", output_format = "html_document")
```

Or from the command line:

```bash
Rscript -e 'rmarkdown::render("Week1.Rmd")'
```

---

## Author

- **Eric Schmidt** ([@telpirion](https://github.com/telpirion))

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
