# Sales Analysis

E-Commerce Marketing Campaign

## Table of Contents

- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools](#tools)
- [Data Cleaning](#data-cleaning)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Results](#results)
- [Recommendations](#recommendations)
- [Limitations](#limitations)
- [References](#references)


### Project Overview

This project evaluates the impact of a marketing campaign using A/B testing on an e-commerce dataset. The goal is to determine whether exposing users to ads significantly improves conversion rates compared to a control group that saw either a public service announcement (PSA) or nothing. The analysis involves hypothesis testing to assess the statistical significance of any observed differences and to estimate potential revenue gains.



### Data Sources

The dataset contains the following fields:

- Row index

- User ID

- Test group ("ad" for the experimental group, "psa" for the control group)

- Converted (True/False indicating if a user converted)

- Total ads seen

- Most ads day

- Most ads hour

### Tools

- Python

- Pandas

- NumPy

= Matplotlib / Seaborn (for visualization)

- Scipy.stats (for statistical testing)

- Jupyter Notebook

### Data Cleaning

- Loaded the dataset and inspected its structure

- Renamed or referenced correct test group labels ("ad" and "psa")

- Checked for missing values and data types

- Ensured the 'converted' column was properly interpreted as boolean

### Exploratory Data Analysis

- Grouped and visualized the distribution of users in the ad and PSA groups

- Analyzed conversion rates across the groups

- Plotted total ads seen distribution

- Investigated trends based on most active day and hour

### Data Analysis

- Separated data into experimental (ad) and control (psa) groups

- Performed a T-test to compare conversion rates

- Calculated estimated revenue:

  -Experimental Group Revenue = Number of conversions * assumed revenue per conversion (e.g., $20)

  -Control Group Revenue = Same formula applied to PSA group

### Results

- Estimated Experimental Group Revenue: $288,460.00

- Estimated Control Group Revenue: $8,400.00

- T-statistic: -7.37

- P-value: 1.70e-13

- Conclusion: The difference in conversion rates is statistically significant (p < 0.05)

### Recommendations

- Continue running targeted ads to improve conversions

- Refine ad content and timing based on most responsive hours/days

- Further segment audience to optimize ROI

### Limitations

- Assumes a fixed revenue per conversion

- No demographic or behavioral segmentation included

- Short time frame may limit generalizability

### References

[scipy-t-test](https://docs.scipy.org/doc/scipy/)

[pandas-library](https://pandas.pydata.org/)

[numPy-library](https://numpy.org/)

