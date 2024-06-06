# TMDb Movie Data Analysis Project

## Overview

This project involves analyzing the TMDb movie dataset, which has been cleaned and prepared for exploration. The main goal is to investigate various aspects of movies, such as release timing, runtime, profitability, and the relationship between different variables such as popularity, budget, revenue, and votes.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Questions Explored](#questions-explored)
- [Data Cleaning](#data-cleaning)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Conclusions](#conclusions)
- [Limitations](#limitations)
- [Requirements](#requirements)
- [Usage](#usage)

## Introduction

The TMDb movie dataset contains information about movies, including their budget, revenue, runtime, cast, director, genres, production companies, release dates, vote counts, and vote averages. This analysis aims to extract meaningful insights from the dataset and answer specific questions related to movie production and success factors.

## Dataset

The dataset used for this analysis is derived from The Movie Database (TMDb) and contains the following columns:

- `id`
- `imdb_id`
- `popularity`
- `budget`
- `revenue`
- `original_title`
- `cast`
- `homepage`
- `director`
- `tagline`
- `keywords`
- `overview`
- `runtime`
- `genres`
- `production_companies`
- `release_date`
- `vote_count`
- `vote_average`
- `release_year`
- `budget_adj`
- `revenue_adj`

## Questions Explored

1. What is the best month to publish a movie?
2. What is the average runtime of films?
3. What are the profits and budgets for each year, and what is the relationship between them?
4. What are the top 10 most profitable films?
5. What is the relationship between vote average and popularity?
6. What is the relationship between popularity and profit?

## Data Cleaning

Several steps were taken to clean the dataset, including:

- Removing duplicate rows.
- Handling missing values.
- Converting data types, such as changing the `release_date` to datetime format.
- Creating new columns, such as extracting `year`, `month`, and `day` from the `release_date`.
- Calculating profits by subtracting the budget from the revenue.

## Exploratory Data Analysis

The analysis included:

1. **Best Month to Publish a Movie**:
   - Calculated total profits for each month.
   - Identified June as the most profitable month for movie releases.

2. **Average Runtime of Films**:
   - Calculated the average runtime of movies, which is approximately 102 minutes.

3. **Profits and Budgets Each Year**:
   - Analyzed the total profits and budgets over the years.
   - Found a positive correlation (0.54) between profit and budget.

4. **Top 10 Most Profitable Films**:
   - Identified the top 10 movies with the highest profits.

5. **Relationship Between Vote Average and Popularity**:
   - Determined a weak positive correlation (0.21) between vote average and popularity.

6. **Relationship Between Popularity and Profit**:
   - Found a moderate positive correlation (0.60) between popularity and profit.

## Conclusions

1. The average movie viewing time is approximately 102 minutes.
2. The most profitable films are generally released in June.
3. There is a moderate positive correlation between popularity and profit.
4. There is a weak positive correlation between vote average and popularity.
5. There is a moderate positive correlation between profit and budget.

## Limitations

- The dataset may not be entirely accurate or up-to-date.
- The budget and revenue columns do not specify currency units, which could affect profit calculations due to currency differences.
- Assumptions about currency types (e.g., USD, Yen) could introduce significant discrepancies in the profit analysis.

## Requirements

To run the analysis, you need the following Python packages:

- pandas
- numpy
- matplotlib
- seaborn

## Usage

1. Clone the repository to your local machine.
2. Ensure you have the required Python packages installed.
3. Load the dataset and run the analysis scripts to generate insights and visualizations.

This project provides a comprehensive exploration of the TMDb movie dataset, offering valuable insights for understanding movie industry trends and factors contributing to movie success.
