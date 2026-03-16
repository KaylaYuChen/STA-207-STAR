## RPUB
https://rpubs.com/kyachen/STA207Project


## Overview
This project analyzes data from **Project STAR (Student/Teacher Achievement Ratio)**, one of the largest randomized education experiments conducted in the United States. The study evaluates whether **smaller class sizes improve early reading outcomes** and whether these effects differ across socioeconomic groups.

Using statistical modeling and causal inference techniques, this analysis estimates the impact of classroom size on reading scores for **kindergarten and first-grade students**.

---

## Abstract
This study examines whether smaller class sizes improve early reading outcomes using data from Project STAR, a randomized experiment conducted in Tennessee. Students entering kindergarten were randomly assigned to one of three classroom types: small classes, regular classes, or regular classes with a teacher’s aide. Because assignment occurred randomly within schools, the design allows causal effects of class size to be estimated.

Using mixed-effects ANOVA and regression models, this analysis evaluates the effect of class size on reading scores in kindergarten and first grade while controlling for race, free-lunch status, and school-level variation.

Results show that students in small classes score higher on average than students in regular classes. The difference is approximately **6 points in kindergarten** and increases to about **14 points in first grade**. However, socioeconomic factors such as free-lunch status remain strong predictors of student achievement. Overall, the findings suggest that smaller class sizes improve early reading outcomes but do not fully eliminate achievement gaps.

---

## Background
Project STAR was a large randomized education experiment conducted in Tennessee in the mid-1980s. Students entering kindergarten were randomly assigned to one of three classroom types:

- **Small classes**
- **Regular classes**
- **Regular classes with a teacher’s aide**

Random assignment occurred **within schools**, meaning students attending the same school were randomly placed into different classroom types. Because of this design, treatment assignment is independent of student background characteristics, allowing causal effects of class size on student outcomes to be estimated.

This analysis focuses on **reading scores** as the primary outcome variable. Early reading ability is widely considered a foundational academic skill that supports later academic development.

---

## Research Questions

### Primary Question
Does assignment to **small classes** causally improve reading scores?

### Secondary Question
Do students from **lower socioeconomic backgrounds** benefit more from smaller classes?

If smaller classes produce larger benefits for disadvantaged students, reducing class size could help narrow achievement gaps in education.

---

## Methods

The analysis consists of several steps:

1. **Data Cleaning**
   - Removed missing observations
   - Transformed the dataset into long format

2. **Exploratory Data Analysis**
   - Checked distributions of reading scores
   - Verified treatment balance across groups

3. **Mixed Effects ANOVA**
   - Estimated class size effects
   - Included school as a random effect

4. **Regression Modeling**
   - Modeled reading scores using:
     - class size
     - free lunch status
     - race
     - school variation

5. **Sensitivity Analysis**
   - Matching analysis
   - Change-in-score model

---

## Key Findings

- Students in **small classes perform better** on reading tests.
- The effect increases from **~6 points in kindergarten** to **~14 points in first grade**.
- **Socioeconomic status (free lunch)** is the strongest predictor of reading outcomes.
- **School differences** also contribute to variation in performance.

Overall, smaller class sizes improve reading outcomes, but **socioeconomic inequalities remain a major factor in educational achievement**.

---

## Tools Used

This project was implemented using **R** and the following packages:

- `tidyverse`
- `ggplot2`
- `lme4`
- `emmeans`
- `MatchIt`
- `plotly`

---

## Authors
- Kayla Yu Chen 
- Jack La
- Matthew Martinez
- Kevin Zhou 
