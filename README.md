# 2024 Medicaid Core Set Quality Measures: State-Level Analysis


**View the Interactive HTML Report Here:** [[Link to your GitHub Pages URL]](https://[YOUR-GITHUB-USERNAME].github.io/[YOUR-REPO-NAME]/)


## Project Overview

This repository contains an exploratory policy analysis of the 2024 Child and Adult Health Care Quality Measures dataset, encompassing 52 reporting jurisdictions. The project translates 6,400+ state-measure observations into standardized performance metrics to evaluate structural variations in state-level Medicaid administration, with a specific focus on behavioral health, substance use disorder (SUD) care, and geographic disparities.

As prevention research increasingly relies on understanding how resources and interventions are delivered to communities, this analysis seeks to identify where Medicaid administrative frameworks succeed and where transparency gaps obscure care quality.


## Key Findings

1. **The Transparency Deficit:** Approximately 10% of reported values are suppressed or hidden. Critical behavioral health metrics, notably *Depression Screening*, suffer from universal "Not Publicly Reported" statuses, acting as systemic black holes in care oversight.

2. **Geographic Inequity:** Standardized composite Z-scoring reveals a stark geographic divide, with Northeast jurisdictions significantly outperforming the South in overall care quality delivery.

3. **The Pediatric/Adult Chasm:** Structural advantages exist for pediatric care across nearly all states. Child follow-up rates post-mental health hospitalization outpace adult rates by an average of 12 percentage points.

4. **Extreme Volatility in SUD Care:** Measures relating to Substance Use Disorder (SUD) and Opioid Use Disorder (OUD) exhibit the most volatile state-to-state variance, ranging from 0.3% to 89.6%.


## Methodology & Tools

This project was built entirely in **R** and compiled using **R Markdown** to ensure complete reproducibility. 

* **Data Processing:** `dplyr` and `tidyr` were utilized to clean suppression codes, handle missingness programmatically, and calculate composite Z-scores across disparate measures.

* **Visualization:** Publication-ready visualizations were developed using `ggplot2` and `ggrepel`, employing a custom, hex-coded organizational brand palette to ensure visual consistency.

* **Data Handling:** Non-numeric suppression codes (e.g., `DS`, `NPR`) were retained analytically to quantify reporting completeness rather than silently dropping incomplete data.


## Repository Structure

```text
├── data/
│   └── 2024-health-quality-measures.csv  # Raw CMS dataset (Ensure this is in your repo)
├── index.Rmd                             # The core analytical script and markdown narrative
├── index.html                            # The compiled report hosted via GitHub Pages
└── README.md                             # Project documentation