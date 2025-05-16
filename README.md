# Movielens-Analysis

MovieLens Data Analysis

An exploratory Python notebook that ingests 100,000 MovieLens ratings, engineers year/decade and genre features, and visualizes trends in genre popularity and average ratings over time using pandas and matplotlib.

  Table of Contents

1. Project Overview
2. Dataset Description
3. Installation & Setup
4. Usage
5. Analysis Sections
6. Key Findings
7. Data License & Citation


2. Dataset Description

This project loads and examines the MovieLens CSV files to explore how average movie ratings change across decades and genres. It covers data validation, feature extraction (release year, decade, genre splitting), aggregation of ratings, and creation of visual summaries using pandas and matplotlib.

Source: GroupLens Research, University of Minnesota.

Files:

ratings.csv (100,836 ratings)
movies.csv (9,742 movies)
tags.csv (3,683 tag applications)
links.csv

Timeframe: 1996–2018, user ratings on a 0.5–5.0 star scale.

Fields: userId, movieId, rating, timestamp, title, genres, tag, plus external IDs.

3. Installation & Setup

Clone this repository

git clone https://github.com/your-username/movielens-analysis.git
cd movielens-analysis

Install dependencies

pip install -r requirements.txt

Launch Jupyter Notebook

jupyter notebook notebooks/movielens_Analysis.ipynb

4. Usage

Run the notebook cells in order to load data, perform sanity checks, feature engineering, and produce charts.

All file paths use relative paths (data/) so the notebook runs on any machine with the same structure.

5. Analysis Sections

- Imports & Sanity Check – verifies data shapes, types, and missing values.

- Feature Engineering – extracts release year and decade, splits genres.

- Movie-Level Analysis – top-rated and most-rated movies, average rating over decades (line chart).

- Genre-Level Analysis – counts and average by genre, scatter/bubble chart of popularity vs. satisfaction.

- Genre×Decade Pivot Table – pivot table of average ratings per genre per decade.

6. Key Findings

1990s Peak: Average ratings peaked in the 1990s (~3.9 stars) and dipped in the 2000s before rebounding.

Popular vs. Niche Genres: Drama and Comedy dominate in volume, while Westerns and Film‑Noir are more niche but highly rated.

Genre Trends: Family/Animation grew steadily; Horror showed lower average satisfaction but high rating count.

7. Data License & Citation

This analysis uses the MovieLens dataset under the GroupLens license. Cite:

Harper, F. M., & Konstan, J. A. (2015). The MovieLens Datasets: History and Context. ACM Transactions on Interactive Intelligent Systems (TiiS), 5(4), 19:1–19:19. https://doi.org/10.1145/2827872
