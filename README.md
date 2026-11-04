# Cumulative Study Guide: Business Statistics with R

A comprehensive, cumulative study guide and computational reference for applied 
business statistics. This repository combines textbook theory, mathematical
formulas, and practical R implementations.

---

## Overview

This repository provides reproducible study materials designed to reinforce core
statistical foundations and their application in R. Each module includes:
- **Conceptual Summaries:** Clear definitions, core business use cases, and
  statistical terminology.
- **Mathematical Formulations:** LaTeX-rendered formulas for descriptive and 
  inferential statistics.
- **R Code Implementations:** Reproducible scripts for data classification,
  descriptive tables, frequency distributions, and visual diagnostics.
- **Interactive Practice:** Applied exercises and self-assessment questions
  available in Jupyter Notebook format.

### Quick Links to Rendered Study Guides

- 📘 [**Week 1 Study Guide (HTML)**](guides/Week1.html) — Introduction to Statistics & Charts and Graphs
- 📘 [**Week 7 Study Guide (HTML)**](guides/Week7.html) — Inferences About Two Populations
- 📓 [**Week 7 Practice & Exercises (Jupyter Notebook)**][week7-nb] — 44 Chapter 10 review questions with full mathematical solutions and 5 applied R exercises

---

## Repository Structure

```text
CumulativeStudyGuide/
├── _quarto.yml               # Quarto configuration (routes preview/render output to guides/)
├── CumulativeStudyGuide.code-workspace
├── data/                     # Datasets for exercises and practical demonstrations
│   ├── home_prices.csv       # Home attributes and selling prices
│   ├── nsalary.csv           # New Mexico social services salary data (rural vs. non-rural)
│   └── tires.csv             # Tire treadwear data (weight loss vs. groove wear)
├── guides/                   # Rendered HTML study guides and supporting web assets
│   ├── Week1.html            # Rendered HTML study guide for Week 1
│   ├── Week1_files/          # Supporting assets and plots for Week 1 HTML
│   ├── Week7.html            # Rendered HTML study guide for Week 7
│   └── Week7_files/          # Supporting assets and dependencies for Week 7 HTML
├── LICENSE                   # Repository license (MIT)
├── README.md                 # Curriculum overview and repository documentation
├── Week1.Rmd                 # Source R Markdown document for Week 1 (Chapters 1 & 2)
├── Week7.ipynb               # Jupyter Notebook with 44 study questions & applied exercises
└── Week7.Rmd                 # Source R Markdown document for Week 7 (Chapter 10)
```

---

## Course & Topic Outline

| Module | Textbook Chapters | Key Topics | Study Materials | R Implementations |
| :--- | :--- | :--- | :--- | :--- |
| **Week 1** | **Ch. 1:** Intro to Statistics<br>**Ch. 2:** Charts & Graphs | • Populations vs. Samples<br>• Levels of Measurement (Nominal, Ordinal, Interval, Ratio)<br>• Frequency distributions, class marks, relative & cumulative frequency<br>• Graphical displays & Pareto analysis<br>• Ethical data presentation | • [Source (`Week1.Rmd`)](Week1.Rmd)<br>• [Rendered Guide (`guides/Week1.html`)](guides/Week1.html) | • `factor()` / ordered factors<br>• Frequency tables (`cut()`, `table()`)<br>• `hist()`, frequency polygon, ogive<br>• `stripchart()` dot plots & `stem()`<br>• `barplot()`, `pie()`, & Pareto charts<br>• Two-variable `plot()` with `lm()` regression line |
| **Week 7** | **Ch. 10:** Inferences About Two Populations | • Test selection framework<br>• Difference in two means ($\sigma$ known vs. unknown)<br>• Pooled vs. Welch's unequal-variance $t$-tests<br>• Matched-pairs / related populations<br>• Two-proportion $z$-tests & pooling<br>• Two-variance $F$-tests<br>• Ethical comparative analysis | • [Source (`Week7.Rmd`)](Week7.Rmd)<br>• [Rendered Guide (`guides/Week7.html`)](guides/Week7.html)<br>• [Practice Notebook (`Week7.ipynb`)](Week7.ipynb) | • Custom `two_sample_z_test()`<br>• `t.test(..., var.equal = TRUE)`<br>• `t.test(..., var.equal = FALSE)`<br>• `t.test(..., paired = TRUE)`<br>• `prop.test(..., correct = FALSE)`<br>• `var.test()` |

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

Each study guide is authored in R Markdown (`.Rmd`) and configured to compile into a standalone HTML report with a floating table of contents in the `guides/` directory.

To render via the R console:

```r
# Render Week 1
rmarkdown::render("Week1.Rmd", output_dir = "guides")

# Render Week 7 (uses custom knit hook targeting guides/)
rmarkdown::render("Week7.Rmd", output_dir = "guides")
```

Or from the command line:

```bash
Rscript -e 'rmarkdown::render("Week1.Rmd", output_dir = "guides")'
Rscript -e 'rmarkdown::render("Week7.Rmd", output_dir = "guides")'
```

Using Positron or Quarto CLI:

```bash
quarto render Week7.Rmd
```

---

## Author

- **Eric Schmidt** ([@telpirion](https://github.com/telpirion))

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

week7-nb: https://colab.research.google.com/github/telpirion/CumulativeStudyGuide/blob/main/Week7.ipynb