# Education Project

> This project investigates inequality in educational opportunity among U.S. high schools by examining how average student performance on standardized exams (ACT/SAT) relates to socioeconomic factors.

---

## Project Overview

This project explores the relationship between school performance on college entrance exams and socioeconomic conditions. Using national education datasets, we aim to uncover whether disparities in student achievement align with differences in economic and demographic backgrounds.

- **Objective:** To determine whether school-level ACT and SAT performance correlates with socioeconomic factors such as income level, or living in married family, thereby revealing patterns of educational inequality.
- **Domain:** Education and Social Science / Public Policy
- **Key Techniques:** Data Cleaning, Data Integration, Exploratory Data Analysis (EDA), Correlation Analysis, Visualization, and Time Series.

---

## Project Structure

```
├── data/                                   # Raw and processed data
├──── ccd_sch_029_1617_w_1a_11212017.csv    # school information data
├──── EdGap_data.xlsx                       # EdGap data
├──── education_clean.csv                   # Cleaned combination of EdGap and School information data
├── code/                                   # Jupyter notebooks and Python scripts
├──── Education.ipynb                       # Jupyter notebook for prepare and process data
├── reports/                                # Generated reports and visualizations
├── requirements.txt                        # Dependencies
└── README.md                               # Project documentation
```

---

## Data

- **Source:**
  1. [EdGap Data](https://github.com/brian-fischer/DATA-5100/blob/main/EdGap_data.xlsx)
  2. [School Information](https://www.dropbox.com/scl/fi/fkafjk8902sq8ptxh94r2/ccd_sch_029_1617_w_1a_11212017.csv?rlkey=gucrdz5f6e38bezz2y3yalxbw&dl=0)
- **Description:**
  The EdGap Data provides information on average ACT and SAT scores across U.S. high schools, including key performance indicators by school ID. It captures academic achievement data that serve as a measure of educational opportunity.
  The School Information Dataset (CCD data) contains demographic and institutional details about each school—such as school name, district, location, enrollment, and other socioeconomic indicators.
  Together, these datasets enable a comparative analysis of school performance relative to socioeconomic conditions.
  - File Format: Excel (.xlsx) and CSV (.csv)
  - Size: Each file contains tens of thousands of rows representing high schools across the U.S.
  - Key Variables: School identifiers (NCESSCH), average ACT/SAT scores, location, and demographic metrics.
- **License:** (if applicable)

### Data Preparation

1. Steps Taken to Prepare the Data
   The raw education datasets were imported, inspected, and cleaned to ensure consistent structure and valid school identifiers. Key preparation steps included:

   - Importing the EdGap dataset (data/EdGap_data.xlsx) and the CCD School Information dataset (data/ccd_sch_029_1617_w_1a_11212017.csv).
   - Inspecting both datasets for missing values and inconsistent identifiers.
   - Cleaning and standardizing the school ID (id/NCESSCH) fields by converting all IDs to strings, trimming spaces, and ensuring consistent digit length to prevent mismatches.
   - Performing an left join to merge the two datasets, preserving all records for completeness.
   - Reviewing the merged data for missing information and applying imputation or filtering where appropriate.
   - Exporting the cleaned datasets for use in subsequent analysis and visualization tasks.

2. The resulting cleaned data files used for analysis are:
   - education_clean.csv

---

## Analysis

Describe the notebooks and/or scripts used to perform the analysis. Specify the order in which the code should be run to reproduce the results.

---

## Results

Include a short discussion of the findings and what they imply.

---

## Authors

- Cong Ho - [@TheCong07](https://github.com/TheCong07)

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Acknowledgements

- Tools/libraries used
- Tutorials or papers referenced
- Inspiration or collaborators
