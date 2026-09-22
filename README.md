# Vaccination Data Analysis and Visualization

## Project Overview

This project analyzes vaccination coverage, disease incidence, reported cases, vaccine introduction, and vaccination schedules across countries and regions. The project was completed using Python for data cleaning and EDA, SQL for database organization, and Power BI for the final dashboard visualization.

## Project Type
EDA (Exploratory Data Analysis)

## Contribution
Individual Project

## Objectives

- Clean and understand vaccination-related datasets
- Analyze vaccination coverage and disease trends
- Compare countries and regions
- Study reported cases and disease incidence
- Analyze vaccine introduction and vaccination schedules
- Perform statistical and correlation analysis
- Create a normalized SQL database
- Present the main findings through a Power BI dashboard

## Datasets

The project uses five datasets:

- Coverage Data
- Incidence Rate Data
- Reported Cases Data
- Vaccine Introduction Data
- Vaccine Schedule Data

The datasets contain information about countries, regions, vaccines, diseases, years, vaccination coverage, reported cases, incidence rates, and vaccination schedules.

## Data Cleaning

The datasets were inspected and cleaned using Python. The work included checking missing values, duplicate records, data types, structural footer rows, invalid values, negative dose values, coverage values above 100, country-level and aggregate records, and different incidence denominators.

Missing values were retained where they represented unavailable source information. Invalid dose values were flagged, and coverage values above 100 were identified rather than blindly modifying the original source data.

## Exploratory Data Analysis

The analysis includes:

- Vaccination coverage analysis
- Disease incidence analysis
- Reported cases analysis
- Country-level comparisons
- Regional comparisons
- Year-wise trends
- Descriptive statistics
- Correlation analysis

## Statistical Analysis

The main correlation analysis focused on MCV1 vaccination coverage and measles incidence using compatible country-year observations.

- Paired observations: 7,280
- Pearson correlation: -0.2144
- Spearman correlation: -0.4870

The results show an inverse association between MCV1 vaccination coverage and measles incidence in the analyzed data. The correlation represents an association and does not establish causation.

## SQL Database

A normalized SQLite database was created to organize the cleaned data.

### Dimension Tables
- `dim_country`
- `dim_vaccine`
- `dim_disease`
- `dim_year`

### Fact Tables
- `fact_coverage`
- `fact_incidence`
- `fact_cases`
- `fact_vaccine_introduction`
- `fact_vaccine_schedule`

The database was checked for primary-key and foreign-key integrity.

## Power BI Dashboard

A Power BI Desktop dashboard was created to present the main project findings.

The dashboard contains:

- KPI cards for Average Vaccination Coverage
- KPI card for Total Reported Cases
- KPI card for Vaccine Introduction Records
- Vaccination Coverage Trend by Year
- Top 10 Countries by Reported Cases
- Vaccination Coverage vs Disease Incidence scatter plot
- Geographic vaccination coverage map
- Country slicer
- Year slicer

The final dashboard was created and saved as a Power BI Desktop `.pbix` file.

## Key Findings

- Vaccination coverage varies across countries and years.
- Reported cases and disease incidence show differences across geographic areas.
- Later-dose coverage generally shows a drop compared with the first dose in the available data.
- Vaccine introduction years vary across countries and regions.
- MCV1 vaccination coverage showed an inverse association with measles incidence in the analyzed observations.
- Several requested variables such as gender, education, urban/rural status, population density, socioeconomic information, and monthly seasonality were not available in the supplied datasets.

## Limitations

The analysis is limited by missing information in some source datasets. Reported cases should also be interpreted carefully because population size and reporting differences can affect raw case counts. Different incidence denominators were kept separate to avoid inappropriate comparisons.

## Project Workflow

`Data Collection → Data Inspection → Data Cleaning → Data Wrangling → EDA → Statistical Analysis → SQL Database → Power BI Dashboard → Insights`

## Technologies Used

Python • Pandas • NumPy • Matplotlib • Seaborn • SQLite • SQL • Power BI • Jupyter Notebook • Google Colab • GitHub

## Project Files

The repository contains the project notebook, source datasets, cleaned/SQL table CSV files, SQLite database, Power BI `.pbix` dashboard, and project documentation.

## Author

**Priyadharshini**

M.Sc. Computer Science

GitHub: https://github.com/Priyadh1/vaccination_project
