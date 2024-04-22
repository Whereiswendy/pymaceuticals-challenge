# pymaceuticals-challenge
UWA Data Analytics Bootcamp Module 5 Challenge using Pandas Matplotlib Scipy Numpy

# Module 5 Challenge
This is the challenge content provided

## Overview

**Due**: Monday by 23:59  
**Points**: 100  
**Submission**: Text entry box or website URL  

**Question**: What good is data without a good plot to tell the story?

In this assignment, you will apply what you've learned about Matplotlib to a real-world situation and dataset involving the pharmaceutical company, Pymaceuticals, Inc., which specializes in anti-cancer medications. Your task is to generate tables and figures for the clinical study of potential treatments for squamous cell carcinoma (SCC).

## Background

You've just joined Pymaceuticals, Inc., a burgeoning pharmaceutical company that has begun screening potential treatments for SCC, a commonly occurring form of skin cancer. 

As a senior data analyst, you have been given access to the complete data from their latest animal study involving 249 mice identified with SCC tumors, treated with various drug regimens over 45 days. Your goal is to analyze and compare the performance of Pymaceuticals' drug of interest, Capomulin, against other treatment regimens.

The executive team has tasked you with generating all of the tables and figures needed for the technical report of the clinical study. They have also asked you for a top-level summary of the study results.

## Files
Download the following files to help you get started:
- [Module 5 Challenge Files](https://static.bc-edx.com/data/dl-1-2/m5/lms/starter/Starter_Code.zip)

## Instructions
This assignment is broken down into the following tasks:

- Prepare the data.

- Generate summary statistics.

- Create bar charts and pie charts.

- Calculate quartiles, find outliers, and create a box plot.

- Create a line plot and a scatter plot.

- Calculate correlation and regression.

- Submit your final analysis.

### Prepare the Data
1. Run the provided package dependency and data imports.
2. Merge the `mouse_metadata` and `study_results` DataFrames into a single DataFrame.
3. Display the number of unique mice IDs, check for duplicate IDs and remove them.
4. Use the cleaned DataFrame for further analysis.

### Generate Summary Statistics
Create a DataFrame of summary statistics. Remember, there is more than one method to produce the results you're after, so the method you use is less important than the result.

Your summary statistics should include:

- A row for each drug regimen. These regimen names should be contained in the index column.

- A column for each of the following statistics: mean, median, variance, standard deviation, and SEM of the tumor volume.

### Create Bar and Pie Charts
1. Generate two bar charts. Both charts should be identical and show the total total number of rows (Mouse ID/Timepoints) for each drug regimen throughout the study.

    - Create the first bar chart with the Pandas `DataFrame.plot()` method.

    - Create the second bar chart with Matplotlib's `pyplot` methods.

2. Generate two pie charts. Both charts should be identical and show the distribution of female versus male mice in the study.

    - Create the first pie chart with the Pandas `DataFrame.plot()` method.

    - Create the second pie chart with Matplotlib's `pyplot` methods.

### Calculate Quartiles, Find Outliers, and Create a Box Plot
1. Calculate the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Then, calculate the quartiles and IQR, and determine if there are any potential outliers across all four treatment regimens. Use the following substeps:

    - Create a grouped DataFrame that shows the last (greatest) time point for each mouse. Merge this grouped DataFrame with the original cleaned DataFrame.

    - Create a list that holds the treatment names as well as a second, empty list to hold the tumor volume data.

    - Loop through each drug in the treatment list, locating the rows in the merged DataFrame that correspond to each treatment. Append the resulting final tumor volumes for each drug to the empty list.

    - Determine outliers by using the upper and lower bounds, and then print the results.

2. Using Matplotlib, generate a box plot that shows the distribution of the final tumor volume for all the mice in each treatment group. Highlight any potential outliers in the plot by changing their color and style.

**hint:** All four box plots should be within the same figure. Use this Matplotlib documentation pageLinks to an external site. for help with changing the style of the outliers.

### Create a Line Plot and a Scatter Plot
1. Select a single mouse that was treated with Capomulin, and generate a line plot of tumor volume versus time point for that mouse.

2. Generate a scatter plot of mouse weight versus average observed tumor volume for the entire Capomulin treatment regimen.

### Calculate Correlation and Regression
1. Calculate the correlation coefficient and linear regression model between mouse weight and average observed tumor volume for the entire Capomulin treatment regimen.

2. Plot the linear regression model on top of the previous scatter plot.

## Requirements

## Prepare the Data (20 points)
- **Merge the datasets into a single DataFrame.** (6 points)
- **Display the number of mice from the merged DataFrame.** (2 points)
- **Identify each duplicate mouse based on the Mouse ID and Timepoint.** (6 points)
- **Create a clean DataFrame with the dropped duplicate mice.** (4 points)
- **Display the number of mice from the clean DataFrame.** (2 points)

## Generate Summary Statistics (15 points)
- **Calculate the mean of the tumor volume for each regimen using `groupby`.** (2 points)
- **Calculate the median of the tumor volume for each regimen using `groupby`.** (2 points)
- **Calculate the variance of the tumor volume for each regimen using `groupby`.** (2 points)
- **Calculate the standard deviation of the tumor volume for each regimen using `groupby`.** (2 points)
- **Calculate the SEM of the tumor volume for each regimen using `groupby`.** (2 points)
- **Create a new DataFrame using the summary statistics.** (5 points)

## Create Bar Charts and Pie Charts (15 points)
- **Generate a bar plot showing the total number of timepoints for all mice tested for each drug regimen using Pandas.** (4.5 points)
- **Generate a bar plot showing the total number of timepoints for all mice tested for each drug regimen using pyplot.** (4.5 points)
- **Generate a pie plot showing the distribution of female versus male mice using Pandas.** (3 points)
- **Generate a pie plot showing the distribution of female versus male mice using pyplot.** (3 points)

## Calculate Quartiles, Find Outliers, and Create a Box Plot (30 points)
- **Create a DataFrame that has the last timepoint for each mouse ID using `groupby`.** (5 points)
- **Reset the index of the DataFrame.** (2 points)
- **Retrieve the maximum timepoint for each mouse.** (2 points)
- **List the four treatment groups (Capomulin, Ramicane, Infubinol, and Ceftamin).** (3 points)
- **Create an empty list to hold tumor volume data.** (3 points)
- **Use a for loop to display the interquartile range (IQR) and identify outliers for each treatment group.** (10 points)
- **Generate a box plot that shows the distribution of the final tumor volume for all the mice in each treatment group.** (5 points)

## Create a Line Plot and a Scatter Plot (10 points)
- **Generate a line plot showing the tumor volume vs. time point for one mouse treated with Capomulin.** (5 points)
- **Generate a scatter plot showing average tumor volume vs. mouse weight for the Capomulin regimen.** (5 points)

## Calculate Correlation and Regression (10 points)
- **Calculate the correlation coefficient and linear regression model for mouse weight and average observed tumor volume for the Capomulin regimen.** (10 points)

## Grading
This assignment will be evaluated against the requirements and assigned a grade according to the following table:

| Grade    | Points |
|----------|--------|
| A (+/-)  | 90+    |
| B (+/-)  | 80–89  |
| C (+/-)  | 70–79  |
| D (+/-)  | 60–69  |
| F (+/-)  | < 60   |


## Submission

To submit your challenge assignment, provide the URL of your GitHub repository. Ensure all plots, tables, and necessary documentation are included and clearly visible in your repository.

## Important Notes

- Remember to credit any code sources or collaborations in your README.
- Utilize the hints and documentation provided to guide your completion of this challenge.

## Support Services

If you need help:
- Use the class Slack channel for peer support.
- Contact BCS Learning Assistants via your class Slack.
- Attend office hours with your instructional staff.

---

*Data generated by Mockaroo, LLC (2022). Realistic Data Generator.*
