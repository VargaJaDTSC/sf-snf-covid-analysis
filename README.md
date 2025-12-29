# sf-snf-covid-analysis
Exploratory analysis of San Francisco County skilled nursing facility COVID-19 data from the California Open Data Portal.

## Overview
This project is an exploratory data analysis (EDA) of COVID-19 infection
data reported by skilled nursing facilities (SNFs) in San Francisco County.
The analysis focuses on facility-level patterns, visualization, and correlation
between resident and health care worker COVID-19 case counts.

The dataset used in this project covers all of California, however, this analysis
is focused specifically on San Francisco County.

## Data
The dataset includes cumulative, facility-level COVID-19 reporting data, such as:
- Total resident COVID-19 infections and deaths
- Total health care worker COVID-19 infections and deaths
- Facility identifiers, county, and reporting dates

The data contain missing values (NaN) and represent cumulative counts reported
over time.

## Methods
The analysis includes:
- Exploratory data analysis and descriptive statistics
- Data cleaning and handling of missing values
- Aggregation to facility-level cumulative totals
- Visualization of case distributions across facilities
- Identification and exclusion of a dominant outlier for comparative analysis
- Correlation analysis between resident and health care worker case counts

Formal hypothesis testing (e.g., t-tests, ANOVA, chi-square) was not conducted due
to skewed distributions, substantial missing data, and the absence of clearly
defined comparison groups.

## Key Findings
- COVID-19 case counts across San Francisco SNFs are highly right-skewed, driven
  primarily by Laguna Honda Hospital & Rehabilitation Center.
- Approximately 79% of facilities reported zero cumulative resident COVID-19
  deaths, limiting the usefulness of death-based analyses.
- After cleaning the data and excluding the dominant outlier, a strong positive
  correlation (r ≈ 0.92) was observed between total resident and total health care
  worker COVID-19 case counts.
- Observed associations do not imply causation and should be interpreted with
  caution given data limitations.

## Limitations
- Facility-level COVID-19 death data appear limited.
- The analysis is observational and descriptive in nature.
- Cumulative reporting limits the ability to assess when increases in infections occurred
  or whether changes in resident and health care worker case counts happened in which
  order.

## Future Work
Future analyses could:
- Compare San Francisco County with other California counties
- Incorporate facility-level characteristics such as bed capacity, staffing
  levels, or visitation policies
- Explore time-series patterns in COVID-19 case reporting

## Data Source
California Open Data Portal (data.ca.gov).
Dataset: "Covid-19 Skilled Nursing Facility Data" (California Department of Public Health).
Accessed: 2025-10-1

Source URL:
https://data.ca.gov/dataset/covid-19-skilled-nursing-facility-data

## Notes
This project is intended for educational and exploratory purposes.
