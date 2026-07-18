# Netflix Data - Exploratory Data Analysis (EDA)

## Problem Statement
Analyze the Netflix content dataset to identify trends and patterns, 
such as content type distribution, year-wise content addition, and 
top content-producing countries.

## Dataset Details
- **Source:** Kaggle (Netflix Movies and TV Shows Dataset)
  URL: https://www.kaggle.com/code/lucifierx/netflix
- **Rows:** 8807
- **Columns:** 12 (show_id, type, title, director, cast, country, date_added, 
  release_year, rating, duration, listed_in, description)

## Approach
1. Loaded the dataset and checked basic info (shape, data types)
2. Checked for missing values
3. Generated summary statistics
4. Created visualizations:
   - Movies vs TV Shows count
   - Year-wise content addition trend
   - Top 10 countries by content count
   - Correlation heatmap (release_year vs year_added)

## Results
- Movies (6131) significantly outnumber TV Shows (2676)
- 2019 saw the highest amount of content added to Netflix
- The United States is the largest content producer (~2800 titles), 
  followed by India (~1000)
- There is a weak correlation (0.11) between release_year and year_added

## Tools Used
- Python, Pandas, NumPy, Matplotlib, Seaborn