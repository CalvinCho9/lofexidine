# Importance of Systolic Blood Pressure in MHOWS as an Evaluation of Lofexidine Efficacy  
### Duke Department of Statistical Science – Undergraduate Research in Statistics Workshop (Summer 2024)
### Project collaborators + mentoring listed on finalpaper.pdf

## Overview  
This project was completed as part of Duke University’s **Undergraduate Research in Statistics Workshop**, a two-week mentored research experience organized by the **Department of Statistical Science** through the **Trinity Research Enhancement Grant**.  
The program aimed to give undergraduates early exposure to research in statistical science and reproducible R workflows.

Our team focused on analyzing the **efficacy of Lofexidine**, an α2-adrenergic receptor agonist, in treating **opioid withdrawal symptoms**. We used open clinical trial data (NIDA-CSP-1020) to examine how including **systolic blood pressure (SYS)** in the Modified Himmelsbach Opiate Withdrawal Scale (**MHOWS**) affects the interpretation of Lofexidine’s effectiveness.

---

## Objective  
To evaluate whether the inclusion of **systolic blood pressure** in MHOWS alters the perceived efficacy of Lofexidine in reducing opioid withdrawal symptoms.

---

## Dataset & Methods  
- **Dataset:** National Institute on Drug Abuse (NIDA-CSP-1020) clinical trial  
- **Sample Size:** 68 opioid-dependent participants (Lofexidine vs. placebo)  
- **Primary Metric:** MHOWS score on Study Day 5  
- **Tools:** `R`, `tidyverse`, `tidymodels`, `glmnet`, `ggplot2`, `rms`  
- **Approach:**  
  - Cleaned and merged NIH clinical CSVs (IMC01–IMC27)  
  - Reconstructed MHOWS scores *with* and *without* systolic BP  
  - Ran multiple and lasso regression models  
  - Conducted cross-validation and residual diagnostics  
  - Created multi-panel visualizations comparing withdrawal trends

---

## Key Findings  
- Including systolic blood pressure in MHOWS **decreased withdrawal scores** for the Lofexidine group.  
- Excluding it **reversed the trend**, showing **higher MHOWS scores** in the Lofexidine group compared to placebo.  
- This indicates that **Lofexidine’s primary effect** may stem from its **blood-pressure-lowering properties** rather than comprehensive withdrawal relief.  
- The results suggest the need for **combination therapies** addressing both physiological and psychological withdrawal symptoms.

---

## Significance  
This project highlights the importance of **variable decomposition** in clinical research and demonstrates how physiological measures like blood pressure can **bias treatment efficacy metrics**.  
It provides a reproducible example of **open-data reanalysis** at the intersection of **biostatistics**, **pharmacology**, and **data science**.
