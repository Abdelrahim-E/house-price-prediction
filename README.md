# House price prediction

Predicts house sale prices from the Kaggle "House Prices - Advanced Regression Techniques" dataset. This is a practice project.

## What I did
- Cleaned the missing values. Most gaps meant the house has no pool, alley or garage, so I filled them with "None" or 0 instead of dropping rows.
- Plotted price against size and quality, and checked which features link most to price.
- Removed 2 outliers (very large houses that sold cheaply).
- Trained Linear Regression and a Decision Tree on an 80/20 split.

## Results
| Model | RMSE | R² |
| --- | --- | --- |
| Linear Regression | $23,153 | 0.898 |
| Decision Tree | $40,563 | 0.686 |

Overall quality and living area are the two features most linked to price.

## Limits
One train/test split, no tuning, no cross-validation. These are first results.

## Run it yourself
1. Download `train.csv` from the [Kaggle competition](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data) and put it next to the notebook.
2. Open `house_price_analysis.ipynb` in Jupyter and run all cells.

Tools: Python, Pandas, Matplotlib, Seaborn, scikit-learn.