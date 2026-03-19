# Olympics Medals Prediction Using Linear Regression

This repository presents a data-driven analysis to predict the number of medals a country will win in the Olympics by leveraging historical athlete data and aggregated team performance.

## Dataset
This project utilizes two primary datasets to bridge the gap between individual athlete performance and national success:

1. **`athlete_events.csv`**
   - **Source:** [Kaggle – 120 Years of Olympic History](https://www.kaggle.com/datasets/heesoo37/120-years-of-olympic-history-athletes-and-results)
   - **Description:** Raw athlete-level data containing 271,116 records.
   - **Variables:** `ID`, `Name`, `Sex`, `Age`, `Height`, `Weight`, `Team`, `NOC`, `Games`, `Year`, `Season`, `City`, `Sport`, `Event`, and `Medal`.

2. **`teams.csv`**
   - **Description:** Processed and aggregated version of the raw data, focused on team-level statistics per Olympic year.
   - **Variables:** `team`, `country`, `year`, `events`, `athletes`, `age`, `height`, `weight`, `medals`, `prev_medals`, and `prev_3_medals`.
   - **Purpose:** Used as the primary input for training the predictive model.

## Clone Repository
```bash
git clone https://github.com/mragilsa/olympics-medals-prediction.git
```

## Install Dependencies
```bash
pip install pandas seaborn scikit-learn matplotlib
```

## Run Notebook
```
olympics-medals-prediction.ipynb
```

## Conclusion
This analysis evaluates the predictability of Olympic success using a Linear Regression model. The findings indicate that a country's past performance `(prev_medals)` and the size of its delegation `(athletes)` are the strongest predictors of future success. The model achieved a low error ratio for powerhouse nations, confirming that Olympic excellence is often consistent and trend-based.
