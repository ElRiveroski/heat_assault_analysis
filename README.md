# heat_assault_analysis
Exploratory data analysis and correlation modeling of temperature vs aggravated assault arrests across 10 U.S. states, including regression, state-level comparisons, and distribution analysis.

## Video Walkthrough

This video provides a full explanation of:
- Data collection (Census, FBI, NOAA)
- Data cleaning and preprocessing
- Visualization and regression analysis
- Key findings and limitations

Watch here: https://youtu.be/Rzi-2wpbAG8

## Overview

This project analyzes the relationship between temperature and aggravated assault arrests across the 10 most populous U.S. states from February 2024 through February 2026.

The goal is to evaluate whether environmental factors—specifically temperature—have a measurable impact on human behavior, particularly violent incidents.


## Key Questions

* Does higher temperature lead to more aggravated assaults?
* Do relationships vary by state?
* Does temperature variability matter more than absolute temperature?


## Data Sources

* **U.S. Census Bureau** — Population data
* **FBI Crime Data Explorer** — Aggravated assault data
* **NOAA / NCEI Climate at a Glance** — Maximum temperature data


## Methodology

* Data cleaning and transformation using `pandas`
* Reshaping datasets into long format for analysis
* Time alignment across datasets 
* Filtering to February 2024 – February 2026
* Merging assault and weather datasets
* Correlation analysis (overall and by state)
* Linear regression modeling
* Data visualization using `matplotlib`


## Key Results

* **Overall correlation:** weak positive relationship *(r ≈ 0.28)*
* Strong positive correlations observed in:

  * New York *(r ≈ 0.84)*
  * North Carolina *(r ≈ 0.82)*
  * Pennsylvania *(r ≈ 0.80)*
* Several states show weak or negative relationships:

  * Texas *(r ≈ -0.50)*
  * California *(r ≈ -0.24)*

### Interpretation

* Temperature alone is not a strong predictor of aggravated assault arrests.
* Temperature variability, rather than absolute temperature, appears more influential.
* In consistently hot states, extreme heat may reduce activity, limiting opportunities for conflict.



## Limitations

* Statewide temperature averages are **highly smoothed**
* Minimal temperature variation reduces statistical sensitivity
* Does not account for:

  * Population density differences
  * Policing strategies
  * Socioeconomic factors
  * Urban vs rural variation


## Future Work

* Use **city-level or daily temperature data**
* Incorporate **heat index / humidity**
* Add demographic and socioeconomic variables
* Apply **multivariate regression models**


## Tech Stack

* Python
* pandas
* matplotlib
* NumPy


## Author

Rolando Rivera
GitHub: https://github.com/ElRiveroski

