# ABC Company — Employee Workforce & Salary Analysis

## Project Overview
This project presents an exploratory data analysis (EDA) of ABC Company's workforce dataset.

## Dataset Description
- Columns: `Name`, `Team`, `Number`, `Position`, `Age`, `Height`, `Weight`, `College`, `Salary`
-  Distribution: 30 teams across 5 positions (`PG`, `SG`, `SF`, `PF`, `C`)

## Preprocessing Steps
- **Missing Value Removal:** Dropped rows containing missing (`NaN`) values and reset the index cleanly.
- **Height Column Replacement:** Replaced the `Height` column with `365` randomly generated integer values between `150` and `180`  and cast the values as `int64`.
- **Duplicate Check:** Verified row uniqueness with `data.duplicated().value_counts()`, confirming `0` duplicate records across all `365` rows.

## Analysis Tasks & Graphical Representations
- **Employee Distribution by Team (Horizontal Bar Chart):** Evaluated headcount and percentage share across all 30 teams.
- **Employee Distribution by Position (Pie Chart):** Analyzed workforce breakdown across `SG`, `PF`, `PG`, `SF`, and `C`.
- **Age Distribution (Scatter Plot):** Examined employee headcount across ages `19` to `40`.
- **Salary Expenditure Distribution (3-Panel Subplot Dashboard):** Compared maximum salary across:
  1. `Team` and `Position` combined
  2. `Team` as a whole
  3. `Position` as a whole
- **Correlation Analysis (Annotated Heatmap):** Computed pairwise correlation (`corr()`) across numeric variables (`Number`, `Age`, `Height`, `Weight`, `Salary`).


## Key Insights & Data Story
Employee headcount is evenly balanced across all 30 teams (8 to 16 employees per team) and largely consistent across core positions (SG, PF, PG, and SF around 19.5%–23.8%, with C smallest at 13.7%), while ages form a right-skewed profile peaking around 24–25 before tapering off after age 32. Maximum salaries reach nearly 22.9M (SF on the New York Knicks) and step down across teams and positions, with individual teams able to hold multiple top-paying roles at different tiers. Meanwhile, numeric correlations across the dataset are weak overall (-0.16 to 0.24), including only a weak positive link between Age and Salary (0.16). Together, these patterns show a young, evenly staffed organization where peak compensation is shaped more by team and position than by age or linear numeric trends.



## Repository Contents
- Project overview, preprocessing summary, visualizations, and insights
- Formatted Jupyter Notebook containing all Python code, charts, and markdown explanations
- Dataset used for the analysis


## Tools & Libraries Used
- **Python 3**, **Jupyter Notebook**
- **Pandas & Numpy** (data manipulation and aggregation)
- **Matplotlib & Seaborn** (data visualization)
