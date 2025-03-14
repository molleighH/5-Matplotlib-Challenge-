# Module 5 Challenge: Pymaceuticals - Data Analysis and Visualization

## Project Overview

In this challenge, I applied my skills in data preparation, summary statistics, data visualization, and statistical analysis using Python and Matplotlib to analyze data from a clinical study conducted by Pymaceuticals, Inc. The goal of the study was to assess the effectiveness of various drug regimens, including Capomulin, in treating squamous cell carcinoma (SCC), a form of skin cancer, in mice. The dataset consists of tumor volume measurements taken over 45 days from 249 mice, each treated with different drug regimens.

As a senior data analyst, I was tasked with generating the necessary tables, figures, and a summary of the study results to contribute to the technical report for the executive team.

## Files

- **`mouse_metadata.csv`**: Contains metadata about the mice, including their ID and gender.
- **`study_results.csv`**: Contains the tumor measurements over time for each mouse.
- **`analysis/`**: Directory containing the output files of the analysis.
- **`README.md`**: This file, providing an overview of the project and analysis.

## Instructions

### 1. Prepare the Data
I began by merging the `mouse_metadata` and `study_results` DataFrames into a single DataFrame. I then:
- Displayed the number of unique mice IDs.
- Identified and removed any duplicate time points for a specific mouse, ensuring clean data for further analysis.
- Checked the number of unique mice IDs in the cleaned dataset.

### 2. Generate Summary Statistics
Using the cleaned dataset, I calculated summary statistics for each drug regimen, including:
- Mean, median, variance, standard deviation, and standard error of the mean (SEM) of the tumor volume.

This was achieved using the `groupby` function to group the data by drug regimen and compute the required statistics.

### 3. Create Bar Charts and Pie Charts
I visualized the following:
- **Bar Charts**: 
  - The total number of timepoints for each drug regimen, created both with Pandas `plot()` and Matplotlib's `pyplot`.
- **Pie Charts**:
  - The distribution of male versus female mice in the study, also created using both Pandas `plot()` and Matplotlib's `pyplot`.

### 4. Calculate Quartiles, Find Outliers, and Create a Box Plot
- I calculated the final tumor volume for each mouse and focused on the four most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin.
- I used the interquartile range (IQR) to detect potential outliers for each treatment regimen.
- A box plot was generated to visualize the distribution of final tumor volumes for each drug regimen, with outliers clearly highlighted.

### 5. Create a Line Plot and a Scatter Plot
- A **line plot** was created for a single mouse treated with Capomulin, showing tumor volume over time.
- A **scatter plot** was generated to show the relationship between mouse weight and average tumor volume for the entire Capomulin treatment group.

### 6. Calculate Correlation and Regression
- I calculated the **correlation coefficient** between mouse weight and average tumor volume for the Capomulin regimen.
- A **linear regression model** was fitted, and the results were plotted on the scatter plot.

## Analysis and Observations

From the analysis, the following key observations were made:
1. **Effectiveness of Capomulin**: The Capomulin regimen consistently showed lower tumor volume growth compared to other treatments.
2. **Correlation between Mouse Weight and Tumor Volume**: A positive correlation was found between mouse weight and average tumor volume, suggesting that heavier mice tend to have larger tumor volumes.
3. **Outliers in Tumor Volume**: Potential outliers were identified in the tumor volume data for the treatment regimens, especially for Infubinol, where a significant variation in tumor volume was observed.

## Requirements Summary

- **Data Preparation**: Merged and cleaned the data, removed duplicate timepoints, and displayed the number of unique mice IDs.
- **Summary Statistics**: Calculated mean, median, variance, standard deviation, and SEM for tumor volume by regimen.
- **Visualizations**: Created bar and pie charts using both Pandas and Matplotlib.
- **Box Plot**: Generated a box plot to show the distribution of tumor volumes and identified outliers.
- **Line and Scatter Plots**: Created a line plot for a single mouse and a scatter plot for tumor volume vs. mouse weight.
- **Correlation and Regression**: Calculated the correlation coefficient and fitted a regression model between mouse weight and tumor volume.

## Tools Used
- **Python** (Pandas, Matplotlib, SciPy)
- **Jupyter Notebooks** for analysis and documentation

## Conclusion

This analysis demonstrates the power of data visualization and statistical methods in understanding and interpreting experimental results. The insights gained from this study will help guide Pymaceuticals in making data-driven decisions regarding the efficacy of their drug regimens.


