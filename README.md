# Census Income Data Visualization

## Project Overview

This project analyzes the UCI Adult Census Income dataset to explore demographic and socioeconomic factors associated with annual income.

The goal of the analysis is to compare individuals earning:

- `<=50K`
- `>50K`

and examine which variables appear to be related to income.

This project was completed as part of the CSE 578 Data Visualization course.

## Dataset

The project uses the UCI Adult Census Income dataset.

The dataset contains 32,561 records and includes variables such as:

- Age
- Workclass
- Education
- Marital status
- Occupation
- Race
- Sex
- Capital gain
- Capital loss
- Hours worked per week
- Native country
- Income

The main target variable is `income`, which separates individuals into two groups:

- `<=50K`
- `>50K`

## Data Cleaning

Before creating the visualizations, the dataset was cleaned using Python and Pandas.

The main cleaning steps included:

- Assigning column names to the raw dataset
- Removing leading and trailing whitespace from categorical values
- Replacing `?` values with missing values
- Creating a cleaned DataFrame for further analysis
- Reviewing unique values in each column

## Exploratory Analysis

Several scenarios were explored to investigate possible relationships between demographic variables and income.

### Scenario 1: Workclass and Income

The relationship between workclass and income was analyzed.

Income was converted into binary values:

- `<=50K` = 0
- `>50K` = 1

The data was grouped by workclass, and the average was used to calculate the percentage of individuals earning more than $50K in each workclass category.

A bar chart was then used to compare these percentages.

### Scenario 2: Age, Capital Gain, Hours Worked, and Income

A parallel coordinates plot was used to compare:

- Age
- Capital gain
- Hours worked per week
- Income group

Rows with zero capital gain were excluded from this particular visualization to make differences among non-zero capital-gain values easier to observe.

A sample of the data was used to reduce visual clutter.

### Scenario 3: Race, Hours Worked, and Income

A categorical point plot was used to compare average hours worked per week across race categories.

Income was used as a grouping variable to compare:

- Individuals earning `<=50K`
- Individuals earning `>50K`

This visualization helped examine whether working-hour patterns differed across race and income groups.

### Scenario 4: Age, Capital Gain, and Income

A scatter plot was created to examine the relationship between age and capital gain.

Each point represents an individual, while color is used to distinguish between the two income groups.

This visualization was used to explore whether age and capital gain show different patterns for individuals earning above and below $50K.

### Scenario 5: Capital Gain Distribution and Income

The distribution of capital gain was compared between the two income groups.

Because many individuals have zero capital gain, the analysis focused on non-zero capital-gain values to make the distribution easier to interpret.

A distribution plot was used to compare the two income groups.

## Tools and Libraries

The project was completed using:

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Plotly
- Jupyter Notebook

## Files

- `project.ipynb` - Main analysis and visualizations
- `Appendix.ipynb` - Additional project code
- `adult.data` - Adult Census Income dataset
- `adult.names` - Dataset attribute descriptions

## Project Goal

The overall goal of the project was to use data visualization to identify patterns that may help explain which demographic and socioeconomic factors are associated with earning more than $50,000 per year.
