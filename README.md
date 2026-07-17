# YES Bank Stock Price Analysis

This project was completed as part of the **Data Science with AI Internship at LABMENTIX**. It analyzes historical YES Bank stock prices and builds machine learning regression models to predict the closing stock price.

## Business Objective

The objective is to understand YES Bank's stock price behavior, identify trends and volatility, and build a predictive model that can estimate the closing price from historical price features.

## Dataset

The dataset contains monthly YES Bank stock prices from **Jul-2005 to Nov-2020**.

Columns:

- `Date`
- `Open`
- `High`
- `Low`
- `Close`

Dataset location:

- `data/raw/yes_bank_stock_prices.csv`

## Project Structure

```text
YES-Bank-Stock-Price-Analysis/
├── README.md
├── START_HERE.md
├── requirements.txt
├── data/
│   ├── README.md
│   └── raw/
│       └── yes_bank_stock_prices.csv
├── models/
│   └── best_stock_price_model.pkl
├── notebooks/
│   ├── 01_eda_yes_bank_stock_price_analysis.ipynb
│   └── 02_ml_yes_bank_stock_price_prediction.ipynb
└── reports/
    ├── yes_bank_presentation.pptx
    └── figures/
        ├── eda/
        └── ml/
```

## Exploratory Data Analysis

The EDA notebook includes:

- Data loading and inspection
- Missing value check
- Duplicate value check
- Date conversion
- Feature engineering with year and month
- Statistical summary
- Trend analysis
- Correlation analysis
- Distribution analysis
- Outlier detection
- Monthly and yearly visualizations

Notebook:

- `notebooks/01_eda_yes_bank_stock_price_analysis.ipynb`

## Machine Learning

The ML notebook trains and compares regression models:

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor

Evaluation metrics:

- MAE
- MSE
- RMSE
- R2 Score

The Random Forest Regressor was selected as the final model and saved to:

- `models/best_stock_price_model.pkl`

Notebook:

- `notebooks/02_ml_yes_bank_stock_price_prediction.ipynb`

## Key Insights

- The dataset has 185 rows and 5 columns.
- There are no missing values or duplicate rows.
- Open, High, Low, and Close prices are strongly positively correlated.
- YES Bank stock prices rose strongly until around 2018.
- Prices declined sharply after 2018.
- High volatility and outliers are visible in several periods.

## How To Run

Create an environment and install dependencies:

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook
```

Run the notebooks in this order:

1. `notebooks/01_eda_yes_bank_stock_price_analysis.ipynb`
2. `notebooks/02_ml_yes_bank_stock_price_prediction.ipynb`

## Final Deliverables

- EDA notebook
- ML notebook
- Cleaned project README
- Dataset
- Saved machine learning model
- Presentation
- Visualization screenshots

## Note

This project is for educational purposes. Stock price prediction is affected by market news, company performance, economic conditions, and investor sentiment, so this model should not be used as real investment advice.
