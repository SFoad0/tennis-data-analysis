#  Tennis Match Data Analysis

This project focuses on the exploration and analysis of a professional tennis dataset. The goal is to extract meaningful insights about players, match performance, and trends using both raw and processed data files.

The analysis is guided by a set of 23 questions, covering various aspects such as player statistics, match duration, win rates, and more.


##  Project Structure

```

tennis-data-analysis/
├── data/
│   ├── tennis_data_20231212/       # Raw data in Parquet format, organized by category
│   └── dataset_csv/                # Preprocessed CSV files for each data source
├── notebooks/
│   ├── readtennis.ipynb            # Converts raw Parquet files into CSV format
│   └── tennis.ipynb                # Main analysis notebook
└── README.md

```



##  Data Preparation

Before starting the analysis, the raw data (in Parquet format) was converted into structured CSV files for easier manipulation. Steps include:

1. **Reading & Converting**: Used PyArrow and Pandas to convert `.parquet` files into `.csv` using `readtennis.ipynb`.
2. **Cleaning**:
   - Removed duplicate records
   - Handled missing values
   - Ensured consistent data types (e.g. integers, floats, categories)
3. **Merging**: Joined datasets where necessary using match IDs and player names.



##  Sample Analysis Questions

The project investigates 23 detailed analytical questions. Here are a few examples:

1. **How many tennis players are included in the dataset?**
2. **What is the average age of the players?**
3. **Which player has the highest number of wins?**
4. **What is the longest match recorded in terms of duration?**

Further questions include:

- What are the most frequent final scores?
- Is there a pattern in match wins based on player ranking?
- How often do players win after losing the first set?
- What is the win ratio for left-handed vs right-handed players?
- How does the number of aces relate to match wins?
- Do home players perform better statistically?
- How often are tie-breaks involved in matches?

... and many more insights based on point-by-point and match-level statistics.



##  Tools & Technologies

- Python 3.10+
- Jupyter Notebook
- Pandas & NumPy
- Matplotlib & Seaborn




##  Notes

* This project is part of a data analysis mentorship program.
* All datasets are included in the `/data` folder.
* The raw data is in Parquet format and can be converted to CSV via `readtennis.ipynb`.




