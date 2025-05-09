# Valorant Map Win Correlation Analysis

This project is focused on analyzing **which in-game statistics are most strongly correlated with winning a map** in Valorant, specifically using match data from **Champions 2024**.

## 🔍 Objective

The goal of this project is to explore the relationship between player and team performance metrics (such as ACS, K/D, first kills, etc.) and map outcomes. By identifying which stats correlate most closely with map wins, we hope to gain insight into what truly impacts victory in high-level competitive Valorant.

## 🛠️ Work Environment

This project is being developed in **Google Colab**, which allows for quick prototyping and data manipulation in a cloud-based notebook environment.

## 🗂️ Data Preparation Process

This project required manual data gathering from **VLR.gg**, as there is no official public API (or at least a free or accessible one) for extracting detailed match statistics. The process involved:

1. **Copying and pasting the "map/stats" table** from each match page on VLR.gg.
2. Converting the pasted tables into CSV format using an **online CSV converter**, https://www.convertcsv.com/html-table-to-csv.htm.
3. Loading each CSV into individual pandas DataFrames.
4. Cleaning and formatting each DataFrame to ensure consistent structure and data types.
5. Combining all cleaned DataFrames into one main dataset for analysis.

> ⚠️ Note: This approach is manual and somewhat time-consuming, but it allowed me to collect detailed round-by-round and player-by-player statistics for each map.

## 📓 Notebook: Data Concatenation

The notebook **`valorant_data_concatenation_(champs_2024).ipynb`** is provided to show the exact steps taken to:
- Import and clean each individual CSV (representing one map's stats)
- Combine all of them into a single master DataFrame

This file is **not the final analysis**, but rather a utility script to prepare the data for further exploration.

## 🚧 Work in Progress

This project is currently a **work in progress**. So far, the focus has been on data gathering and cleanup. The **data analysis phase will begin soon**, where I will:
- Explore statistical correlations
- Create visualizations to highlight performance patterns
- Potentially build predictive models to estimate map win probability based on player stats

## 📌 Requirements

- Python 3.x
- pandas
- matplotlib / seaborn (for visualization in later stages)

---

Feel free to explore the notebook and leave feedback or suggestions!
