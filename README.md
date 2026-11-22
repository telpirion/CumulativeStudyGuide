# Cumulative Study Guide: Business Statistics with R

A comprehensive, cumulative study guide and computational reference for applied 
business statistics. This repository combines textbook theory, mathematical
formulas, and practical R implementations.

> **Disclaimer:** These study materials were compiled by Gemini, with editing by me ([@telpirion](https://github.com/telpirion)).

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
- 📘 [**Week 2 Study Guide (HTML)**](guides/Week2.html) — Descriptive Statistics & Modern Robust Analytics
- 📓 [**Week 2 Practice & Exercises (Jupyter Notebook)**](https://colab.research.google.com/github/telpirion/CumulativeStudyGuide/blob/main/Week2.ipynb) — 41 Chapter 3 review questions with full mathematical solutions and 6 applied R exercises
- 📘 [**Week 3 Study Guide (HTML)**](guides/Week3.html) — Probability, Bayes' Theorem & Discrete Distributions
- 📓 [**Week 3 Practice & Exercises (Jupyter Notebook)**](https://colab.research.google.com/github/telpirion/CumulativeStudyGuide/blob/main/Week3.ipynb) — 41 Chapter 4 & 30 Chapter 5 review questions with full mathematical solutions, plus applied R & Bayesian exercises
- 📘 [**Week 4 Study Guide (HTML)**](guides/Week4.html) — Continuous & Sampling Distributions
- 📓 [**Week 4 Practice & Exercises (Jupyter Notebook)**](https://colab.research.google.com/github/telpirion/CumulativeStudyGuide/blob/main/Week4.ipynb) — 44 Chapter 6 & 28 Chapter 7 review questions with full mathematical solutions, plus 6 applied R exercises
- 📘 [**Week 5 Study Guide (HTML)**](guides/Week5.html) — Statistical Estimation & Modern Robust Intervals
- 📓 [**Week 5 Practice & Exercises (Jupyter Notebook)**](https://colab.research.google.com/github/telpirion/CumulativeStudyGuide/blob/main/Week5.ipynb) — 34 Chapter 8 review questions with full mathematical solutions and 6 applied R exercises
- 📘 [**Week 6 Study Guide (HTML)**](guides/Week6.html) — Hypothesis Testing for Single Populations & Categorical Data Analysis
- 📓 [**Week 6 Practice & Exercises (Jupyter Notebook)**](https://colab.research.google.com/github/telpirion/CumulativeStudyGuide/blob/main/Week6.ipynb) — 50 Chapter 9 & 19 Chapter 16 review questions with full mathematical solutions, plus 12 applied R exercises
- 📘 [**Week 7 Study Guide (HTML)**](guides/Week7.html) — Inferences About Two Populations
- 📓 [**Week 7 Practice & Exercises (Jupyter Notebook)**](https://colab.research.google.com/github/telpirion/CumulativeStudyGuide/blob/main/Week7.ipynb) — 44 Chapter 10 review questions with full mathematical solutions and 5 applied R exercises
- 📘 [**Week 8 Study Guide (HTML)**](guides/Week8.html) — Analysis of Variance & Simple Linear Regression
- 📓 [**Week 8 Practice & Exercises (Jupyter Notebook)**](https://colab.research.google.com/github/telpirion/CumulativeStudyGuide/blob/main/Week8.ipynb) — ANOVA and Regression application exercises and R code examples
- 📘 [**Week 9 Study Guide (HTML)**](guides/Week9.html) — Regression Inference, Diagnostics, Correlation ($r^2$) & Multiple Regression
- 📓 [**Week 9 Practice & Exercises (Jupyter Notebook)**](https://colab.research.google.com/github/telpirion/CumulativeStudyGuide/blob/main/Week9.ipynb) — 36 Chapter 12 & 7 Chapter 13 study questions plus `newspapers`, `tableware`, and R supplement applied exercises

---

## Repository Structure

```text
CumulativeStudyGuide/
├── _quarto.yml               # Quarto configuration (routes preview/render output to guides/)
├── AGENTS.md                 # Repository coding and notebook instructions
├── CumulativeStudyGuide.code-workspace
├── data/                     # Datasets for exercises and practical demonstrations
│   ├── geyser.csv            # Old Faithful Geyser eruption intervals (WEEK1 & WEEK2)
│   ├── home_prices.csv       # Home attributes and selling prices
│   ├── hot_dogs.csv          # Hot dog types, calories, and sodium content (ANOVA & Week 6)
│   ├── mileage.csv           # 1991 US EPA passenger car mileage, HP, and weight classes
│   ├── newspapers.csv        # 1994 Gale Directory daily and Sunday newspaper circulations
│   ├── nsalary.csv           # New Mexico social services salary data (rural vs. non-rural)
│   ├── pontus.csv            # US Presidential inauguration ages and candidate heights
│   ├── salaries.csv          # Forbes CEO age and salary data for 60 small business firms
│   ├── shoppers.csv          # Store customer dollar spending amounts
│   ├── tableware.csv         # Tableware types, polishing times, prices, and rates (ANOVA)
│   └── tires.csv             # Tire treadwear data (weight loss vs. groove wear)
├── guides/                   # Rendered HTML study guides and supporting web assets
│   ├── Week1.html            # Rendered HTML study guide for Week 1
│   ├── Week1_files/          # Supporting assets and plots for Week 1 HTML
│   ├── Week2.html            # Rendered HTML study guide for Week 2
│   ├── Week2_files/          # Supporting assets and plots for Week 2 HTML
│   ├── Week3.html            # Rendered HTML study guide for Week 3
│   ├── Week3_files/          # Supporting assets and plots for Week 3 HTML
│   ├── Week4.html            # Rendered HTML study guide for Week 4 (self-contained)
│   ├── Week5.html            # Rendered HTML study guide for Week 5 (self-contained)
│   ├── Week6.html            # Rendered HTML study guide for Week 6 (self-contained)
│   ├── Week7.html            # Rendered HTML study guide for Week 7
│   ├── Week7_files/          # Supporting assets and dependencies for Week 7 HTML
│   ├── Week8.html            # Rendered HTML study guide for Week 8
│   ├── Week8_files/          # Supporting assets and plots for Week 8 HTML
│   └── Week9.html            # Rendered HTML study guide for Week 9
├── LICENSE                   # Repository license (MIT)
├── README.md                 # Curriculum overview and repository documentation
├── sources/                  # Curriculum slide decks, solution guides, and reference literature
│   ├── Chapter12PracticeProblems.pdf
│   ├── Chapter13PracticeProblems.pdf
│   ├── Exercises.txt
│   ├── Lesson_12_Simple_Regression_Analysis_and_Correlation_Solutions.pdf
│   ├── R supplement to Business Statistics, Ch 12.R
│   └── R supplement to Business Statistics, Ch 13.R
├── Week1.Rmd                 # Source R Markdown document for Week 1 (Chapters 1 & 2)
├── Week2.ipynb               # Jupyter Notebook with 41 study questions & 6 applied exercises
├── Week2.Rmd                 # Source R Markdown document for Week 2 (Chapter 3)
├── Week3.ipynb               # R Jupyter Notebook with 71 study questions & 3 applied exercises
├── Week3.Rmd                 # Source R Markdown document for Week 3 (Chapters 4 & 5)
├── Week4.ipynb               # R Jupyter Notebook with 72 study questions & 6 applied exercises
├── Week4.Rmd                 # Source R Markdown document for Week 4 (Chapters 6 & 7, Wilcox 4.7)
├── Week5.ipynb               # R Jupyter Notebook with 34 study questions & 6 applied exercises
├── Week5.Rmd                 # Source R Markdown document for Week 5 (Chapter 8, Wilcox 6.5)
├── Week6.ipynb               # R Jupyter Notebook with 69 study questions & 12 applied exercises
├── Week6.Rmd                 # Source R Markdown document for Week 6 (Chapters 9 & 16)
├── Week7.ipynb               # Jupyter Notebook with 44 study questions & applied exercises
├── Week7.Rmd                 # Source R Markdown document for Week 7 (Chapter 10)
├── Week8.ipynb               # Jupyter Notebook with ANOVA/Regression exercises
├── Week8.Rmd                 # Source R Markdown document for Week 8 (Chapters 11 & 12)
├── Week9.ipynb               # R Jupyter Notebook with 43 study questions & 9 applied exercises
└── Week9.Rmd                 # Source R Markdown document for Week 9 (Ch. 12.4–12.9, Wilcox 8.3 & Ch. 13)
```

---

## Course & Topic Outline

| Module | Textbook Chapters | Key Topics | Study Materials | R Implementations |
| :--- | :--- | :--- | :--- | :--- |
| **Week 1** | **Ch. 1:** Intro to Statistics<br>**Ch. 2:** Charts & Graphs | • Populations vs. Samples<br>• Levels of Measurement (Nominal, Ordinal, Interval, Ratio)<br>• Frequency distributions, class marks, relative & cumulative frequency<br>• Graphical displays & Pareto analysis<br>• Ethical data presentation | • [Source (`Week1.Rmd`)](Week1.Rmd)<br>• [Rendered Guide (`guides/Week1.html`)](guides/Week1.html) | • `factor()` / ordered factors<br>• Frequency tables (`cut()`, `table()`)<br>• `hist()`, frequency polygon, ogive<br>• `stripchart()` dot plots & `stem()`<br>• `barplot()`, `pie()`, & Pareto charts<br>• Two-variable `plot()` with `lm()` regression line |
| **Week 2** | **Ch. 3:** Descriptive Statistics | • Central Tendency (Mean, Median, Mode, Trimmed Mean)<br>• Dispersion (Range, $IQR$, MAD, Variance, Standard Deviation, $CV$)<br>• Grouped Data Central Tendency & Variance<br>• Chebyshev's Theorem vs. The Empirical Rule<br>• Shape (Skewness, Kurtosis) & Tukey Outlier Fences<br>• Wilcox Masking & Winsorized Variance<br>• Pearson's Correlation ($r$) | • [Source (`Week2.Rmd`)](Week2.Rmd)<br>• [Rendered Guide (`guides/Week2.html`)](guides/Week2.html)<br>• [Practice Notebook (`Week2.ipynb`)](Week2.ipynb) | • `mean(..., trim = 0.2)`, `median()`, `table()`<br>• `quantile(..., type = 6)`, `IQR()`, `diff(range())`<br>• `var()`, `sd()`, custom `calc_winsorized_var()`<br>• Grouped $\bar{x}$ & $s^2$ calculations<br>• `boxplot(..., horizontal = TRUE)`<br>• `cor()`, `cor.test()`, `plot()` with `lm()`<br>• Applied analyses (`mileage`, `shoppers`, `pontus`, `geyser`) |
| **Week 3** | **Ch. 4:** Probability<br>**Ch. 5:** Discrete Distributions<br>**Think Bayes Ch. 1–2** | • Classical, Relative Frequency & Subjective Probability<br>• Counting Rules ($mn$ rule, Combinations)<br>• Set Operations, Addition, Multiplication & Conditional Rules<br>• Independence & Mutually Exclusive Events<br>• Bayes' Theorem (Diachronic & Table Method)<br>• Discrete Expected Value & Variance<br>• Binomial, Poisson & Hypergeometric Distributions | • [Source (`Week3.Rmd`)](Week3.Rmd)<br>• [Rendered Guide (`guides/Week3.html`)](guides/Week3.html)<br>• [Practice Notebook (`Week3.ipynb`)](Week3.ipynb) | • `sample()`, `expand.grid()`, `choose()`, `combn()`<br>• `union()`, `intersect()`, `replicate()`<br>• Custom `bayes_table()` & `discrete_summary()`<br>• `dbinom()`, `pbinom()`, `dpois()`, `ppois()`<br>• `dhyper()`, `phyper()`<br>• Monte Carlo simulations & `ggplot2` PMF charts |
| **Week 4** | **Ch. 6:** Continuous Distributions<br>**Ch. 7:** Sampling & Sampling Distributions<br>**Wilcox Ch. 4.7** | • Continuous Uniform, Normal ($z$) & Exponential Distributions<br>• Normal Approximation to the Binomial ($\pm 0.5$ continuity correction)<br>• Normality Diagnostics (Histograms, Density, Q-Q Plots)<br>• Probability vs. Non-Probability Sampling & Error Types<br>• Central Limit Theorem ($\bar{x}$ & $\hat{p}$) & FPC Factor<br>• Wilcox Contaminated Normal & Log Back-Transformation | • [Source (`Week4.Rmd`)](Week4.Rmd)<br>• [Rendered Guide (`guides/Week4.html`)](guides/Week4.html)<br>• [Practice Notebook (`Week4.ipynb`)](Week4.ipynb) | • `dunif()`, `punif()`, `runif()`<br>• `dnorm()`, `pnorm()`, `qnorm()`, `rnorm()`<br>• `qqnorm()`, `qqline()`, `dexp()`, `pexp()`<br>• `sample()`, `sample.int()`, `set.seed()`, stratified sampling<br>• CLT simulations & `ggplot2` distribution curves |
| **Week 5** | **Ch. 8:** Estimation for Single Populations<br>**Wilcox Ch. 6.5** | • Point vs. Interval Estimates & Probability Coverage ($1 - \alpha$)<br>• Mean CIs ($\sigma$ known $z$-interval, FPC, & $\sigma$ unknown $t$-interval)<br>• One-Sided Confidence Intervals<br>• Proportion CIs (Wald, Agresti-Coull, Wilson Score, Blyth)<br>• Variance ($\sigma^2$) & Standard Deviation ($\sigma$) $\chi^2$ CIs<br>• Minimum Sample Size ($n$) for $\mu$ and $p$<br>• Wilcox 20% Trimmed Mean (Winsorized SE), Bootstrap-$t$ & Percentile Bootstrap | • [Source (`Week5.Rmd`)](Week5.Rmd)<br>• [Rendered Guide (`guides/Week5.html`)](guides/Week5.html)<br>• [Practice Notebook (`Week5.ipynb`)](Week5.ipynb) | • `qnorm()`, `qt()`, `qchisq()`, `ceiling()`<br>• `t.test()` (two-sided & one-sided)<br>• `prop.test()` & Agresti-Coull comparison<br>• Custom `var_conf_int_summary()`, `trim_ci()`, `boot_t_ci()`<br>• `replicate()`, `sample(..., replace = TRUE)`, `quantile()`<br>• Horizontal `boxplot()` & `hot_dogs.csv` analysis |
| **Week 6** | **Ch. 9:** Hypothesis Testing for Single Populations<br>**Ch. 16:** Analysis of Categorical Data | • Eight-step hypothesis testing process & $p$-value method<br>• Type I ($\alpha$), Type II ($\beta$), Power ($1 - \beta$), OC & Power curves<br>• One-sample $z$-test & $t$-test for $\mu$<br>• One-sample proportion $z$-test & variance $\chi^2$-test<br>• Parametric vs. nonparametric methods<br>• $\chi^2$ Goodness-of-Fit & Test of Independence | • [Source (`Week6.Rmd`)](Week6.Rmd)<br>• [Rendered Guide (`guides/Week6.html`)](guides/Week6.html)<br>• [Practice Notebook (`Week6.ipynb`)](Week6.ipynb) | • Custom `one_sample_z_test()` & `one_sample_var_test()`<br>• `t.test()`, `prop.test()`, `pt()`, `pnorm()`<br>• `qchisq()`, `pchisq()`, `chisq.test()`<br>• `ggplot2` Power/OC curves & horizontal boxplots<br>• Applied analyses (`hot_dogs`, `salaries`) |
| **Week 7** | **Ch. 10:** Inferences About Two Populations | • Test selection framework<br>• Difference in two means ($\sigma$ known vs. unknown)<br>• Pooled vs. Welch's unequal-variance $t$-tests<br>• Matched-pairs / related populations<br>• Two-proportion $z$-tests & pooling<br>• Two-variance $F$-tests<br>• Ethical comparative analysis | • [Source (`Week7.Rmd`)](Week7.Rmd)<br>• [Rendered Guide (`guides/Week7.html`)](guides/Week7.html)<br>• [Practice Notebook (`Week7.ipynb`)](Week7.ipynb) | • Custom `two_sample_z_test()`<br>• `t.test(..., var.equal = TRUE)`<br>• `t.test(..., var.equal = FALSE)`<br>• `t.test(..., paired = TRUE)`<br>• `prop.test(..., correct = FALSE)`<br>• `var.test()` |
| **Week 8** | **Ch. 11:** Analysis of Variance<br>**Ch. 12:** Simple Linear Regression | • One-Way ANOVA & partitioning $SS$<br>• Tukey's HSD post-hoc testing<br>• Randomized Block & Two-Way ANOVA<br>• Simple Linear Regression (OLS)<br>• Correlation vs. Regression<br>• Goodness of fit ($R^2$, $s_e$) | • [Source (`Week8.Rmd`)](Week8.Rmd)<br>• [Rendered Guide (`guides/Week8.html`)](guides/Week8.html)<br>• [Practice Notebook (`Week8.ipynb`)](Week8.ipynb) | • `aov()` & `summary(aov())`<br>• `TukeyHSD()`<br>• `lm()`<br>• `summary(lm())`<br>• Residual analysis (`plot(lm())`)<br>• `predict()` |
| **Week 9** | **Ch. 12.4–12.9:** Regression Inference & Forecasting<br>**Wilcox Ch. 8.3:** Correlation & $r^2$<br>**Ch. 13:** Multiple Regression | • Residual diagnostics & LINE assumptions<br>• Slope $t$-test, CI & ANOVA $F$-test equivalence<br>• Confidence vs. Prediction intervals<br>• Trend-line forecasting<br>• Wilcox's 5 distorting features & heteroscedasticity trap<br>• Multiple regression, Adjusted $R^2$, dummy variables, $VIF$ & $\log_{10}$ transformations | • [Source (`Week9.Rmd`)](Week9.Rmd)<br>• [Rendered Guide (`guides/Week9.html`)](guides/Week9.html)<br>• [Practice Notebook (`Week9.ipynb`)](Week9.ipynb) | • `confint()`, `predict(..., interval = ...)`<br>• `cor.test()`, `anova()`, `pf()`, `pt()`<br>• `par(mfrow = c(2, 2)); plot(lm())`<br>• `bartlett.test()`, `MASS::rlm()`<br>• Manual $VIF_j = 1/(1 - R_j^2)$ calculations<br>• Applied analyses (`tableware`, `newspapers`, Airline Cost, Prime Interest Rate) |

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

# Render Week 2 (uses custom knit hook targeting guides/)
rmarkdown::render("Week2.Rmd", output_dir = "guides")

# Render Week 3
rmarkdown::render("Week3.Rmd", output_dir = "guides")

# Render Week 4 (uses custom knit hook targeting guides/)
rmarkdown::render("Week4.Rmd", output_dir = "guides")

# Render Week 5 (uses custom knit hook targeting guides/)
rmarkdown::render("Week5.Rmd", output_dir = "guides")

# Render Week 6 (uses custom knit hook targeting guides/)
rmarkdown::render("Week6.Rmd", output_dir = "guides")

# Render Week 7 (uses custom knit hook targeting guides/)
rmarkdown::render("Week7.Rmd", output_dir = "guides")

# Render Week 8
rmarkdown::render("Week8.Rmd", output_dir = "guides")

# Render Week 9 (uses custom knit hook targeting guides/)
rmarkdown::render("Week9.Rmd", output_dir = "guides")
```

Or from the command line:

```bash
Rscript -e 'rmarkdown::render("Week1.Rmd", output_dir = "guides")'
Rscript -e 'rmarkdown::render("Week2.Rmd", output_dir = "guides")'
Rscript -e 'rmarkdown::render("Week3.Rmd", output_dir = "guides")'
Rscript -e 'rmarkdown::render("Week4.Rmd", output_dir = "guides")'
Rscript -e 'rmarkdown::render("Week5.Rmd", output_dir = "guides")'
Rscript -e 'rmarkdown::render("Week6.Rmd", output_dir = "guides")'
Rscript -e 'rmarkdown::render("Week7.Rmd", output_dir = "guides")'
Rscript -e 'rmarkdown::render("Week8.Rmd", output_dir = "guides")'
Rscript -e 'rmarkdown::render("Week9.Rmd", output_dir = "guides")'
```

Using Positron or Quarto CLI:

```bash
quarto render Week1.Rmd
quarto render Week2.Rmd
quarto render Week3.Rmd
quarto render Week4.Rmd
quarto render Week5.Rmd
quarto render Week6.Rmd
quarto render Week7.Rmd
quarto render Week8.Rmd
quarto render Week9.Rmd
```

---

## Editor

- **Eric Schmidt** ([@telpirion](https://github.com/telpirion))

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
