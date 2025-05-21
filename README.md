# solar-energy_-challenge_week1-

Overview

This project is part of the 10 Academy's AIM Week 0 Challenge. Its objective is to prepare and analyze solar energy data from various countries to assist with region-ranking and decision-making in renewable energy deployment. The work is organized into specific tasks. This README details the steps and deliverables for Task 1 and Task 2.

✅ Task 1: Git & Project Setup

Objective
To set up a proper version-controlled project workspace using Git and GitHub for collaborative and organized development.

Steps Completed

✅ Initialized Git repository

✅ Created .gitignore to exclude unnecessary files (e.g., virtual environments, CSVs, notebook checkpoints)

✅ Set up Python virtual environment (venv) and installed required packages listed in requirements.txt

✅ Created development branches for each task and feature

✅ Successfully merged branches and maintained a clean commit history

✅ Pushed project to GitHub

✅ Task 2: Data Profiling, Cleaning & Exploratory Data Analysis (EDA)

Objective

To profile, clean, and explore the solar dataset of each country to prepare it for downstream analysis and modeling.

Countries Analyzed

Benin

Sierra Leone

Togo

Each country has its own notebook and cleaned dataset stored locally under the data/ folder.

Key Steps Performed

Branch Creation

Created a dedicated branch for each country (e.g., eda-sirraleone)

Notebook Analysis

Notebooks: benin_eda,sirraleone_eda.ipynb, togo_eda.ipynb

Data Profiling

Used df.describe() to generate summary statistics

Used df.isna().sum() to report missing values

Flagged columns with more than 5% null values

Data Cleaning

Identified outliers using Z-score method (|Z| > 3)

Imputed missing values using median where applicable

Exported cleaned datasets to data/<country>_clean.csv

Exploratory Data Analysis (EDA)

Time series plots of GHI, DNI, DHI, and Tamb

Distribution and outlier analysis for sensor and wind readings

Correlation matrix heatmaps

Scatter plots to analyze environmental relationships

Bubble chart to examine GHI vs Tamb with RH or BP

Wind rose plots and histograms for key variables
Cleaning Impact Analysis

Compared ModA and ModB before and after cleaning
Grouped and visualized data based on cleaning flags
✅ Task 3: Cross-Country Comparison
Objective
To synthesize the cleaned datasets from Benin, Sierra Leone, and Togo to identify relative solar potential and key differences across countries.

Branch: compare-countries
Notebook: compare_countries.ipynb

Key Steps Performed

Data Loading
Loaded cleaned CSVs (data/benin_clean.csv, data/sierraleone_clean.csv, data/togo_clean.csv)
Combined datasets with a 'Country' column for unified analysis
Metric Comparison
Created side-by-side boxplots for GHI, DNI, and DHI, colored by country
Generated a summary table comparing mean, median, and standard deviation of GHI, DNI, DHI across countries
Statistical Testing
Performed Kruskal-Wallis test on GHI to assess significant differences (p-value reported)
Key Observations
Summarized findings in a markdown cell with 3 bullet points highlighting actionable insights (e.g., highest GHI, variability)
Bonus Visualization
Created a bar chart ranking countries by average GHI
Git Hygiene
Committed changes with message: Completed Task 3: Cross-country comparison with boxplots, summary table, and statistical testing
Ensured data/ folder remains ignored in .gitignore
Deliverables

Notebook: compare_countries.ipynb
Summary table CSV: data/summary_stats.csv
Visuals: Boxplots and bar chart for GHI, DNI, DHI
KPIs Achieved

Included all three countries in plots
Correctly reported p-values from statistical testing
Provided relevant, actionable insights in markdown
Generated a summary table with mean, median, and standard deviation
