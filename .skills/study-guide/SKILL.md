---
name: study-guide
description: |
  Create two study guide artifacts using the sources in the /source folder. 
  Review all of the materials in the source folder and create or update two
  artifacts: an .Rmd file with the content from the sources and a .ipynb file
  with R code practice problems.
---

# Create week study guide

## Prerequisites

+ Determine whether there is already an .Rmd study guide in the root of the
  project. The study guide will be titled "Week#.Rmd", where the `#` is the
  current week of the course.
+ If you aren't given the current week in the course, ask the user to tell you
  what week this study guide is for.
+ Be sure to read all instructions in AGENTS.md or RULES.md before executing
  this skill.

## Step 1. Review the week's materials.

1.  Review all materials in the `{root}/sources` folder.
2.  For each chunk of data in the sources material, determine whether it is
    core content, a practice problem, or both.

## Step 2. Create the content study guide

1.  If the .Rmd file for the week already exists, open that file. Read the full
    contents.
2.  Review all of the core content fetched from the sources in Step 1. Summarize
    and write a logical study guide from the material.
    + Use the other .Rmd files in this project as examples or templates.
    + Provide R code all equations and their applications. Clearly describe what
      the inputs are for the equations.
      - Use existing material from /sources if available.
      - If no existing material is available, create new R code blocks. Whenever
        possible, use core R libraries and functions.
    + Provide R code for all sample problems mentioned in the text.
    + If an .Rmd file for this week already exists, update the file with the
      core content from sources.
3.  Be sure to `knit` all .Rmd files in the project when you are done.

## Step 3. Create the Jupyter notebook practice problems

1.  If the .ipynb file for the week already existss, open that file. Read the
    full contents.
2.  Review all of the practice problems content from the sources in Step 1.
    Create an aggregated set of pratice problems from the material.
3.  Always set the notebook to use the R runtime.

## Step 4. Update the README

After creating the new study guide materials, update the README.md file to
reference the newly created files.
