# TV Show Ratings Analysis
## Project Overview
This project analyzes data from the entertainment industry, focusing specifically on TV shows during the "Golden Age" of television, which began in 1999 with the release of The Sopranos and is still ongoing. The primary goal of the analysis is to investigate the relationship between the number of votes a TV show receives on IMDb and its rating. The hypothesis is that highly-rated shows released during the "Golden Age" also have the most votes.

## Table of Contents
1. Project Description
2. Data
3. Project Structure
4. Methodology
  - Data Overview
  - Data Preprocessing
  - Data Analysis
5. Conclusion
6. Future Work

## Project Description
In this project, we analyzed a dataset containing records on movies and TV shows. The analysis focused on TV shows released during the "Golden Age" of television (1999 onwards) to test the hypothesis that shows with higher IMDb scores tend to receive more votes. This project simulates the type of tasks you might encounter as a data professional, where you analyze assumptions and provide data-driven insights.

## Data
The dataset used in this project is stored in the file /datasets/movies_and_shows.csv. It contains the following columns:

- name — Name of the actor or director.
- character — Character played (for actors).
- role — The person’s contribution to the title (either as an actor or director).
- title — Title of the movie or show.
- type — Indicates whether the title is a movie or a show.
- genres — List of genres under which the movie or show falls.
- release_year — Year when the movie or show was released.
- imdb_score — IMDb score of the title.
- imdb_votes — Number of votes the title received on IMDb.

## Project Structure
The project is divided into three main stages:

1. Data Overview: Explore the dataset, check the quality of the data, and identify any potential issues.
2. Data Preprocessing: Clean the data by correcting formatting issues, handling missing values, and removing duplicates.
3. Data Analysis: Perform analysis to test the hypothesis by examining the relationship between IMDb scores and the number of votes.

## Methodology
### Data Overview
In the first stage, the dataset was loaded and explored to understand its structure and identify any data quality issues. The initial exploration revealed inconsistencies in column names and the presence of missing values and duplicates.

### Data Preprocessing
Data preprocessing involved the following steps:

- Column Name Cleaning: Corrected column names to follow good naming conventions (e.g., snake_case, lowercase).
- Missing Values: Dropped rows with missing values in critical columns (imdb_score and imdb_votes).
- Duplicates: Removed duplicate rows and corrected implicit duplicates in the type column.

### Data Analysis
- The analysis focused on TV shows released in 1999 or later. The IMDb scores were rounded, and the number of votes was averaged for each score. Outliers were identified and excluded to ensure the averages were meaningful. The final analysis confirmed that shows with higher IMDb scores tend to have more votes, supporting the initial hypothesis.

## Conclusion
The analysis confirms the hypothesis that highly-rated TV shows released during the "Golden Age" of television tend to have the most votes on IMDb. Specifically, the top three scores (7-9) have the highest average number of votes, indicating a strong correlation between high ratings and the number of votes a show receives.

## Future Work
Further analysis could involve:

Expanding the analysis to include movies and compare trends between movies and TV shows.
Exploring other factors that might influence IMDb ratings and votes, such as genre or the presence of certain actors or directors.
Using machine learning models to predict a show's IMDb score or the number of votes based on other features.
