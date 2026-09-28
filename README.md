# IMDB Movie Data — Exploratory Data Analysis

An EDA project on an IMDB dataset of 1,000 movies (2006–2016) using **Python**, **Pandas**, **Matplotlib**, and **Seaborn**, exploring directors, ratings, revenue trends, and the correlation between votes, ratings, and box office performance.

## 📊 About the Dataset

File: `7-IMDB-Movie-Data.csv` — 1,000 rows × 12 columns.

| Column | Description |
|---|---|
| Rank | Movie's rank in the dataset |
| Title | Movie title |
| Genre | Genre(s) of the movie |
| Description | Short plot description |
| Director | Director of the movie |
| Actors | Lead cast members |
| Year | Year of release (2006–2016) |
| runtime(minutes) | Runtime in minutes (renamed from `Runtime (Minutes)`) |
| Rating | IMDB rating |
| Votes | Number of votes |
| revenue(millions) | Box office revenue in millions (renamed from `Revenue (Millions)`) |
| Metascore | Metascore rating |

**Missing values (before cleaning):** `revenue(millions)` had 128 missing values, `Metascore` had 64 — both filled with `0`.

## 🎯 Purpose

To explore what characterizes top-performing movies and directors on IMDB — which directors are most prolific and highest-rated, how revenue and release volume have trended year over year, and how ratings, votes, and revenue relate to each other.

## 🛠️ Approach

1. **Load and inspect** the dataset — shape, head/tail, column data types.
2. **Clean column names** — rename `Revenue (Millions)` → `revenue(millions)` and `Runtime (Minutes)` → `runtime(minutes)`.
3. **Handle missing values** — fill nulls in `revenue(millions)` and `Metascore` with `0`.
4. **Director analysis** — count unique directors, films per director, top 5 by film count, top 5 by average rating.
5. **Rating and revenue analysis** — top-rated movies, top-grossing movies, top movies by Metascore.
6. **Trend analysis** — movies released per year, total revenue per year (line plot, pie chart).
7. **Correlation analysis** — heatmap across all numerical columns.
8. **Visualization** — pie charts, bar charts, scatter plot, line plot, correlation heatmap.

## ❓ Questions Answered

- What do the first and last 5 rows of the dataset look like, and what is its shape?
- Are there any missing values, and what are the column data types?
- How many unique directors are in the dataset?
- How many movies has each director made?
- What are the top 3 highest-rated movies?
- Which director has made the fewest movies?
- Which movies come from the top 5 most prolific directors?
- How much total revenue have the top 5 directors generated?
- What are the top 5 highest-grossing movies?
- What are the top 5 movies by Metascore, and how do their votes compare?
- What's the relationship between votes and Metascore for top movies?
- What is the correlation between Rank, Year, runtime, Rating, Votes, revenue, and Metascore?
- How many movies were released each year, and what was the yearly revenue trend?
- What's the distribution of movie ratings?
- Which directors have the highest average ratings?
- What is the maximum movie runtime in the dataset?
- What proportion of total revenue did each year contribute?

## 🗄️ Tech Stack

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Jupyter Notebook**

## 📁 Repository Structure

```
├── 7_IMDB_Movie_Data.ipynb   # Notebook with code, outputs, and visualizations
├── Project_Report.docx       # Full project report
└── README.md
```

## 🚀 How to Run

1. Install the requirements:
   ```
   pip install pandas numpy matplotlib seaborn jupyter
   ```
2. Place `7-IMDB-Movie-Data.csv` in the working directory (update the file path in the notebook if needed — the original path points to a Google Drive mount).
3. Open and run the notebook:
   ```
   jupyter notebook 7_IMDB_Movie_Data.ipynb
   ```

## 📌 Key Findings

- The dataset covers **1,000 movies** across **644 unique directors** (2006–2016).
- Top 3 highest-rated movies: **The Dark Knight** (2008), **Inception** (2010), and **Dangal** (2016).
- **Nitesh Tiwari** has the highest average rating (**8.80**), followed by **Christopher Nolan** (**8.68**).
- Movie releases grew sharply over time — from **44 movies in 2006** to **297 movies in 2016**.
- Yearly total revenue grew alongside release volume — from **$3,624M in 2006** to **$11,212M in 2016**.
- The maximum runtime in the dataset is **191 minutes**.
- **Zack Snyder** is among the most prolific directors with **5 films** in the dataset.

---
*An exploratory data analysis project on IMDB movie ratings, revenue, and director trends.*
