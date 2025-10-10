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

## Notebooks

- Weather_Data_Preparation_SEA_NYC.ipynb – Prepares the raw precipitation datasets, performs cleaning, handles missing values, and outputs a clean data file.
- Weather_Data_Processing_SEA_NYC.ipynb – Performs the analysis, including exploratory data analysis, visualizations, and hypothesis testing.

---

## Data

- **Source:** [NOAA Climate Data Online (CDO) – Daily Summaries](https://www.ncei.noaa.gov/cdo-web/search?datasetid=GHCND)
- **Description:** Daily precipitation (PRCP) records for Seattle (Sea-Tac Airport station) and New York (Central Park station) covering Jan 1, 2018 – Dec 31, 2022. Data is provided in CSV format and includes station identifiers, dates, and precipitation values (tenths of millimeters).

## Data Preparation

The raw daily precipitation data was downloaded from NOAA’s Climate Data Online (CDO) tool.

### Steps Taken

1. Inspected and downloaded raw NOAA daily precipitation datasets for NY city.
2. Converted data types.
3. Imputed missing precipitation values using day-of-year averages.
4. Saved the cleaned dataset in a tidy long format with consistent column names.

- **Data preparation notebook:** `Weather_Data_Preparation_SEA_NYC.ipynb`
- **Clean data file:** `data/clean_precipitation.csv`

- **License:** (if applicable)

---

## Analysis

- Created derived variables, including any_precipitation, month, and year.
- Produced descriptive statistics and exploratory visualizations using multiple type of graphs and charts to compare rainfall frequency and intensity.
- Conducted hypothesis testing:
  - t-tests to compare average daily precipitation between cities by month.
  - Proportion z-tests to compare the frequency of rainy days between cities by month.
- Interpreted the results to distinguish between rainfall frequency (Seattle higher) and rainfall amount per day (New York higher in some months).

- **Data processing notebook:** `Weather_Data_Processing_SEA_NYC.ipynb`

---

## Results

The analysis helps me answer the question “Does Seattle get more rain than New York?” from two different perspectives:

- First perspective: Seattle has a higher proportion of rainy days than New York in most months, except during the summer (when Seattle has almost no rain). In other words, Seattle rains more frequently.
- Second perspective: Although New York has fewer rainy days than Seattle, the overall picture still shows that New York receives a considerable amount of rainfall over the years. Looking more closely, we can see that New York has some days with rainfall more than double that of Seattle. This indicates that New York often experiences heavy rain events, like storms, but they occur less frequently.

#### Conclusion:

Seattle has more rainy days if we measure by frequency. Meanwhile, if we measure by the average rainfall per rainy day, New York has higher values. To truly answer which city “rains more”, I think we first need to clarify in which sense — frequency or intensity — we are defining “more rain.”

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
