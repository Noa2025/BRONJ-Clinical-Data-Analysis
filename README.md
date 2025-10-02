# Overview
Bisphosphonate-related osteonecrosis of the jaw (BRONJ) is a rare but serious side effect of bisphosphonate therapy, commonly used in cancer patients to prevent bone complications. Understanding risk factors such as demographics, treatment regimens, and genetic predispositions is crucial for early detection and prevention.
This project explores a synthetic dataset modeled after a real clinical trial of cancer patients treated with bisphosphonates. The analysis demonstrates how to integrate multiple data sources (demographics, medications, genetics) into a structured SQLite database and perform statistical testing using Python (pandas, scipy).
Dataset
The dataset consists of 46 cancer patients, all treated with bisphosphonates. Approximately 50% developed BRONJ during the follow-up.
The data is organized into three tables:
## Demographics
* Age
* Gender
* Cancer type
* Race
## Medications
* Type of bisphosphonate
*	Route of administration
*	Duration of treatment
## Genetics
*	Two single-nucleotide polymorphisms (SNP1, SNP2)
# Methods
## Data integration: 
All tables were merged into a single SQLite database (ONJ.db).
## Analysis environment: 
Queries executed in SQL; statistical tests performed in Python using pandas and scipy.
## Statistical analysis:
* Chi-square test (chi2) for categorical variables.
* Student’s t-test (ttest) for continuous variables.
# Results
* SNP1 was significantly associated with BRONJ occurrence (p = 0.049).
* SNP2 was not associated (p = 0.34).
* The combination of SNP1 and SNP2 improved association (p = 0.014).
* Cancer type showed a trend towards association (p = 0.076).
# Tools
* SQLite for structured storage and querying.
* pandas for data manipulation.
* scipy.stats for statistical analysis (chi2, t-test).

