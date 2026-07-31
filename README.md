# Netflix Dataset - Exploratory Data Analysis (EDA)

## 📌 Problem Statement
Netflix has a huge and diverse content library. The goal of this project is to explore the Netflix dataset to identify trends and patterns in the type of content available, such as the split between movies and TV shows, content growth over the years, top content-producing countries, popular genres, content ratings, and typical movie durations.

## 📂 Dataset Details
- **Dataset Name:** Netflix Movies and TV Shows Dataset
- **Source:** Kaggle  Link: https://www.kaggle.com/code/lucifierx/netflix
- **Size:** 8807 rows, 12 columns
- **Key Columns:** `show_id`, `type`, `title`, `director`, `cast`, `country`, `date_added`, `release_year`, `rating`, `duration`, `listed_in`, `description`

## 🛠️ Approach
1. **Data Cleaning**
   - Filled missing values in `director`, `cast`, and `country` with `'Unknown'`
   - Dropped the few rows with missing `date_added`, `rating`, or `duration`
   - Checked and confirmed there were no duplicate rows
   - Final cleaned dataset shape: **(8790, 12)**

2. **Feature Engineering**
   - Converted `date_added` to datetime format
   - Extracted `year_added` and `month_added` columns for trend analysis

3. **Exploratory Data Analysis (EDA)**
   - Summary statistics of the dataset
   - Distribution of Movies vs TV Shows
   - Yearly trend of content added to Netflix
   - Top 10 countries producing content
   - Top 10 genres/categories
   - Distribution of content ratings
   - Correlation analysis between numeric features
   - Movie duration distribution

4. **Visualizations**
   - Bar charts, line chart, heatmap, and histogram created using `matplotlib` and `seaborn`

## 📊 Results / Key Insights
- Netflix's catalog is **movie-heavy**, with 6126 Movies (~70%) vs 2664 TV Shows (~30%)
- Content additions grew rapidly between **2016 and 2019**, peaking around 2019, with a slight drop in 2020-2021
- **United States**, **India**, and **United Kingdom** are the top content-producing countries
- **International Movies**, **Dramas**, and **Comedies** are the most common genres
- Most content is rated **TV-MA** and **TV-14**, indicating a focus on mature/teen audiences
- Numeric features (`release_year`, `year_added`, `month_added`) show **little to no strong correlation**
- Most movies have a runtime between **90 and 120 minutes**

## 🧰 Tools & Libraries Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Vs Code

## 📁 Repository Structure
```
synent-task3-netflixeda-bushrashahid/
│
├── Data/
│   └── netflix_titles.csv
├── netflix_eda.ipynb
└── README.md
```

## ▶️ How to Run
1. Clone this repository
2. Install required libraries: `pip install pandas numpy matplotlib seaborn`
3. Open `netflix_eda.ipynb` in VS Code (with Jupyter extension) or Jupyter Notebook
4. Run all cells

## 👤 Author
Bushra Shahid — Data Science Intern, Synent Technologies
