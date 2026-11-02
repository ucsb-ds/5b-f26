---
layout: default
title: "Project"
nav_order: 9
has_children: true
---
# CMPSC 5B – Final Project

**Fall 2026 – UC Santa Barbara**


## Overview

This is an **individual** project (except as noted in the "Pair Option" section below.) 

You will design and carry out an end-to-end data science investigation using the concepts and techniques covered throughout the course. You will choose one or two real-world datasets, formulate statistical questions, conduct a rigorous analysis, and communicate your findings through a Jupyter Notebook, a slide presentation, and a short video.

The goal is to demonstrate that you can apply the inferential thinking skills from this course to data you care about.

## Pair Option

You are permitted to work in pairs if you wish, but
if you do, you will be responsible for completing four of the extended requirements, instead of just two.

## Library Policy

> **You must use the `datascience` library for all data manipulation and analysis. The use of `pandas` is strictly prohibited and will result in a score of zero for the affected components. You are free the use Matplotlib and Seaborn for visualization purposes.**
> 
> All standard Python libraries (`numpy`, `matplotlib`, `scipy.stats`, etc.) are permitted where appropriate. When in doubt, ask staff.
> 
> Very limited exceptions to this policy may be permitted, but only with advance apprroval.  
>
> For example, we can make an exception for the following use of Pandas: if you need to read from an Excel file directly, you may use the features of Pandas on a limited basis to read in the file, and then convert the Pandas dataframe to a `datascience` file.
> 

## Dataset Requirements

Choose one or two publicly available datasets. A good dataset should:

- Contain at least several hundred rows so that statistical methods are meaningful.
- Have a mix of numeric and categorical variables.
- Require some real cleaning effort (missing values, inconsistent formatting, outliers, etc.).
- Support the statistical analyses described in the Requirements section below.

Ideally, your datasets share a common theme so your notebook tells a coherent story. Using two datasets is fine, but more than two is discouraged, depth matters more than breadth. **The staff provided regular feedback on the datasets you found, so you can continue using the datasets identified so far. If you want to work with new datasets, consult the staff first and get their feedback.**

## Project Requirements

Your analysis must address **all** of the following core requirements and **at least two** of the extended requirements.

### Core Requirements (Required)

1. **Data Cleaning.** Document all cleaning steps explicitly in your notebook. This includes, but is not limited to: handling missing or null values, correcting data types, removing or justifying outliers, standardizing string formats, and filtering rows that are not relevant to your analysis. Explain *why* you made each cleaning decision, not just *what* you did.

2. **Hypothesis Testing.** Formulate and test at least one hypothesis. For each test you must:
   - State the null hypothesis *H*<sub>0</sub> and the alternative hypothesis *H*<sub>A</sub> clearly in plain English.
   - Compute an appropriate test statistic and a p-value.
   - Interpret the p-value in the context of your question. Explain what it does—and does not—tell you. Do not simply state "we reject *H*<sub>0</sub>" without further discussion.
   - State your significance level *α* before conducting the test.

3. **Pearson Correlation and Regression.** Identify two numerical variables from your dataset for which a linear relationship is plausible.
   - Compute the Pearson correlation coefficient *r* and interpret its magnitude and sign.
   - Fit a regression line and display it on a scatter plot.
   - Interpret the slope and intercept in the context of your data.
   - Discuss whether the assumptions of linear regression appear to be reasonably satisfied.

### Extended Requirements (Choose at Least Two)

Choose at least two of the following. You may complete more for a richer analysis.

1. **Comparing an Empirical Sample to an Expected Distribution:** Use simulation to test whether an observed sample is consistent with a known or assumed probability model. Visualize both the observed and expected distributions and compute a p-value using a simulated null distribution.

2. **Comparing Two Empirical Samples:** Compare two groups using a permutation test (or A/B test). State your hypotheses, choose an appropriate test statistic (e.g., difference in means or medians), run the simulation, and interpret the resulting p-value.

3. **Confidence Intervals via Bootstrap:** Construct a 95% bootstrap confidence interval for a statistic of interest (e.g., mean, median, or proportion). Visualize the bootstrap distribution, report the interval, and explain what the interval means in non-technical terms.

4. **Causality and Observational Studies:** Discuss whether your dataset supports causal claims or is purely observational. Identify at least one potential confounding variable. If possible, use a randomized comparison or a matched-pairs argument. Be explicit about the limits of your conclusions.

5. **Prediction and Regression Inference:** Use your regression model to make a prediction for a specific input value. Compute a prediction interval or discuss the uncertainty in the prediction. Evaluate the quality of the model using the residuals.

6. **Classification:** Build and evaluate a simple k-nearest neighbors classifier using the `datascience` library. Split your data into training and test sets, report accuracy, and discuss where the classifier succeeds and where it fails.

## Deliverables

### 1. Jupyter Notebook and GitHub Repository

- Create a GitHub repository containing your Jupyter Notebook and all datasets.
- The notebook must be fully executable from top to bottom without errors. Before submitting, restart the kernel and run all cells.
- Structure the notebook with clear Markdown headers and prose explanations between code cells. Treat it as a written report, not a loose collection of code.
- All figures should have labeled axes and a descriptive title.
- Include a brief introduction section describing your datasets and your research questions, and a conclusion section summarizing your findings.
- The README file in the repository should include: your name, a one-paragraph description of the project, instructions for running the notebook, and a link to each dataset source.

### 2. Slide Presentation

- Prepare a slide deck summarizing your project.
- Suggested structure: title slide, motivation and research questions, dataset description, key findings for each analysis, visualizations, and conclusions.
- Slides should be clear and visually tidy. Do not paste raw code onto slides.

### 3. Video Recording

- Record a short video (5–7 minutes) in which you present your slides and walk through your key results.
- You do not need to appear on camera, but your voice must be audible and clear.
- Upload the video to YouTube (unlisted is fine), Google Drive or another platform accessible without login, and include the link in your GitHub README.

## Deadlines

| Checkpoint | Date | What to Show |
|---|---|---|
| Intermediate Check-in 1: Dataset chosen, repo created, data loaded, high level questions identified  | Friday, Week 6 |
| Intermediate Check-in 2 | Friday, Week 7 | Data cleaning begun, Null and Alternate Hypothesis identified, Pearson Correlation columns identified |
| Intermediate Check-in 3 | Friday, Week 8 | Hypothesis testing and Pearson Correlation completed, including text explanations and interpretation; extended requirements identified.  |
| **Final Submission** | **Friday, June 5, 2026, 11:59 PM** | Complete notebook, slides, and video |

For the intermediate check-ins, you need to have your work reviewed by the instructor or TA.  

For those that complete the step by lecture time  on Wednesday of weeks 6, 7, or 8, they may have the work checked by the instructor or TA in lecture on Wednesday; if they receive a score of 100, they will be excused from Friday section that week.

During Wednesday Lecture or Friday Section, ULAs may also do a preliminary check of the work, and enter a provisional grade into Canvas.  However, this is not final until it is signed off on by a TA or instructor, so if your work is checked by a ULA, please don't leave class until the TA or instructor also looks it over and leaves a comment on the Canvas grade book that it is acceptable.

Each checkpoint contributes 5% of your overall final project grade; the remaining 85% is divided among various criteria (see below)

Grading rubrics for each of the checkpoints will be posted on Canvas.

## Grading Rubric

| Component | Points |
|---|---:|
| Checkpoint 1 | 5 |
| Checkpoint 2 | 5 |
| Checkpoint 3 | 5 |
| Data Cleaning (documentation, justification, completeness) | 10 |
| Hypothesis Testing (setup, computation, interpretation) | 10 |
| Pearson Correlation and Regression | 15 |
| Extended Requirement 1 | 15 |
| Extended Requirement 2 | 15 |
| Notebook quality (structure, prose, reproducibility) | 5 |
| Presentation and Video | 15 |
| **Total** | **100** |


## Academic Integrity

This is an individual project. You may discuss high-level ideas with classmates, but all code, writing, and analysis must be your own. Sharing code, copying from online solutions, or submitting AI-generated notebooks without meaningful personal contribution violates the UCSB Academic Integrity Policy and will be reported.

You are encouraged to use course materials, lecture notes, and the textbook [*Computational and Inferential Thinking*](https://inferentialthinking.com) as references.

## Tips for a Strong Project

- **Choose data you find genuinely interesting.** The more motivated you are, the better your questions will be.
- **Write as you go.** Add Markdown explanations immediately after writing each code cell—do not leave all the writing to the last day.
- **Interpret everything.** A plot or a p-value with no explanation earns minimal credit. What does it mean?
- **Test early.** Restart and re-run your notebook at each checkpoint to make sure it is still reproducible.
- **Come to office hours.** Staff is available to give feedback on your dataset choice and analysis plan before you invest too much time.

---

*Questions? Post on Slack or visit office hours.*

---

Acknowledgments: Ege Demirci (TA for CMPSC 5B, S26) wrote the first version of this file; it was then edited by Phill Conrad.
