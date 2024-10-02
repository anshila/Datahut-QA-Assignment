# Datahut-QA-Assignment

# Data Cleaning Assignment: Employee Records

## Overview

This project focuses on cleaning and analyzing a dataset of employee records. The dataset contains various columns, including employee IDs, names, ages, email addresses, join dates, salaries, and departments. Throughout this assignment, we address multiple data quality issues, such as missing values, inconsistent formatting, outliers, and typographical errors.

## Dataset Description

The dataset includes the following columns:
- **ID**: A unique identifier for each employee.
- **Name**: The employee’s full name.
- **Age**: The employee’s age.
- **Email**: The employee’s email address.
- **Join Date**: The date when the employee joined the company.
- **Salary**: The employee’s salary.
- **Department**: The department the employee works in.

## Data Issues Addressed

1. **Missing Values**: 
   - Some records had missing information, particularly in the *Name*, *Age*, *Email*, *Join Date*, *Salary*, and *Department* columns.
   
2. **Inconsistent Formatting**:
   - Inconsistent capitalization in names.
   - Incorrect or missing date formats in the *Join Date* column.
   
3. **Outliers**:
   - Extreme or implausible values in the *Age* and *Salary* columns.

4. **Typographical Errors**:
   - Typographical errors in department names led to inconsistent categories.

## Data Cleaning Process

### 1. Handling Missing Values:
- **Numerical Columns (Age, Salary)**: Missing values were filled using the median of the respective column.
- **Categorical Columns (Department)**: Missing values were filled with the most frequent category or labeled as "Unknown."

### 2. Standardizing Name Formatting:
- Names were cleaned by ensuring proper capitalization and removing extra characters (e.g., numbers or special symbols).

### 3. Date Formatting:
- The *Join Date* column was cleaned by ensuring a consistent date format. Invalid or missing dates were marked as missing.

### 4. Outlier Detection:
- Outliers in the *Age* and *Salary* columns were identified using statistical methods (e.g., Z-scores or IQR). These outliers were either removed or replaced with more reasonable values (e.g., the median).

### 5. Typographical Fixes for Department:
- The *Department* column was standardized by correcting typographical errors and ensuring consistency (e.g., mapping "Hr" to "HR").

## Assumptions Made

- **Name Cleaning**: It was assumed that extra characters in names (e.g., numbers or symbols) were unintentional errors.
- **Age Range**: Ages outside the range of 18 to 100 were treated as outliers.
- **Salary Outliers**: Salary values that deviated significantly from the norm were assumed to be errors.
- **Missing Join Dates**: Missing or invalid join dates were marked as missing since they were not critical for the analysis.
- **Department Standardization**: Department names were assumed to follow a common format (e.g., "HR" for Human Resources), and variations were treated as typographical errors.

## Conclusion

This project demonstrates a comprehensive approach to data cleaning, addressing common issues such as missing values, inconsistent formatting, and outliers. By applying statistical methods and domain-specific assumptions, we transformed a messy dataset into a more reliable and analyzable format.
