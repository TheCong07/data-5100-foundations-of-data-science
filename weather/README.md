# Weather Project

> This project analyzes and compares precipitation data from Seattle, WA and New York, NY (2018–2022) to evaluate whether Seattle’s reputation as the “rainiest” city is supported by actual data.

---

## Project Overview

- **Objective:** To compare precipitation patterns between Seattle, WA and New York, NY from 2018 to 2022, and test the common belief that Seattle is the “rainiest” city.
- **Domain:** Climate / Environmental Data Analysis
- **Key Techniques:** Time Series analysis, descriptive statistics, and data visualization.

**Summary:**  
The project uses daily precipitation data from NOAA’s Climate Data Online (CDO) tool. Findings show that while Seattle experiences rain more frequently, New York records higher total rainfall over the same period due to heavier, concentrated rain events. This highlights the importance of distinguishing between rainfall frequency and rainfall volume when evaluating “raininess.”

---

## Project Structure

```
├── data/                 # Raw and processed data
├── code/                 # Jupyter notebooks and Python scripts
├── reports/              # Generated reports and visualizations
├── requirements.txt      # Dependencies
└── README.md             # Project documentation
```

---

## Data

- **Source:** [NOAA Climate Data Online (CDO) – Daily Summaries](https://www.ncei.noaa.gov/cdo-web/search?datasetid=GHCND)
- **Description:** Daily precipitation (PRCP) records for Seattle (Sea-Tac Airport station) and New York (Central Park station) covering Jan 1, 2018 – Dec 31, 2022. Data is provided in CSV format and includes station identifiers, dates, and precipitation values (tenths of millimeters).
- **License:** (if applicable)

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
