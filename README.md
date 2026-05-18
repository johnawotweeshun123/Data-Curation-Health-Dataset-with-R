# Data-Curation-Health-Dataset-with-R
Identification of problem, diagnosis, validation and cleaning of a messy health dataset using R.
# Health Data Curation and Quality Diagnosis in R
## Project Overview
This project demonstrates the identifying problems diagnosis, validation, cleaning and management of a messy health dataset using R. The aim was to identify data quality problems and prepare the dataset for future empirical analysis.
## Objectives
The project focused on:
-Identifying problems
- Diagnosing missing values
- Checking duplicate records
- Identifying inconsistent categorical values
- Cleaning numeric variables stored as text
- Validating clinical measurements
- Checking logical inconsistencies
- Creating a cleaned dataset and data quality summary
## Dataset
The dataset contains 2,000 health records and 28 original variables. It includes demographic, clinical, facility, behavioural, and health status variables.
For privacy reasons, the public version of the cleaned dataset excludes patient names.
## Data Quality Issues Identified
The main issues found were:
- Missing values
- Repeated patient IDs
- Inconsistent category coding
- Numeric values recorded with units
- Invalid text entries in numeric variables
- Mixed blood pressure formats
- Invalid age values
- Logical inconsistencies between related variables
## Key Cleaning Steps
The cleaning process included:
- Standardising variable names
- Converting blank entries to missing values
- Standardising categorical variables
- Extracting numeric values from mixed-format variables
- Cleaning and splitting blood pressure into systolic and diastolic values
- Recalculating BMI for validation
- Creating validation flags
- Exporting cleaned data and quality reports
## Main Findings
Some important data quality issues included:
- High glucose but no diabetes: 336 records
- High systolic BP but no hypertension: 222 records
- High diastolic BP but no hypertension: 181 records
- Suspiciously low glucose: 124 records
- Missing BMI information: 108 records
- Male patients with pregnancy-related diagnosis: 99 records
- Missing or non-numeric age: 70 records
## Files in This Repository
| File | Description |
| first group assignment data curation.R | Full reproducible R script |
| health_clean_public.csv | Cleaned anonymised dataset |
| data_quality_summary_updated.csv | Final data quality summary |
| data_management_decisions.csv | Data management decisions |
| missing_summary_after_blank_cleaning.csv | Missing value summary after blank cleaning |
## Tools Used
- R
- tidyverse
- inspectdf
- dplyr
- esquisse
- janitor
- visdat
- skimr
- naniar
- readr
## Reproducibility
All cleaning and validation steps were completed in R. The raw dataset was preserved during analysis and cleaned variables were created separately to ensure transparency and traceability.
