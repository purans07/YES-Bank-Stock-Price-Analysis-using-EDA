# Start Here: YES Bank Stock Price Analysis

## What Data Science with AI Means

Data Science means using data to answer questions and support decisions. In a project, you usually collect data, clean it, explore it with charts, build a model, check model performance, and explain the result.

AI means making a computer perform tasks that normally need human intelligence. In this project, the AI part is Machine Learning: the model learns patterns from old YES Bank stock prices and predicts the closing price.

Simple vocabulary:

- Dataset: the table of data you are analyzing.
- Feature: an input column used by the model, such as Open, High, Low, Year, and Month.
- Target: the output column you want to predict. Here it is Close.
- EDA: Exploratory Data Analysis, where you use summaries and charts to understand the data.
- Regression: a machine learning task where the target is a number.
- Train-test split: training the model on one part of the data and testing it on unseen data.
- MAE/RMSE/R2: metrics used to judge prediction quality.

## What This Project Is Asking You To Do

Your project is to analyze YES Bank monthly stock prices and build a regression model to predict the closing stock price.

The dataset has these columns:

- Date
- Open
- High
- Low
- Close

The main question is: can historical price columns help us understand and predict the closing price?

## Files In This Project

- `data/raw/yes_bank_stock_prices.csv`: the main dataset.
- `notebooks/01_eda_yes_bank_stock_price_analysis.ipynb`: EDA notebook for charts, trends, and business insights.
- `notebooks/02_ml_yes_bank_stock_price_prediction.ipynb`: ML notebook for training and evaluating regression models.
- `models/best_stock_price_model.pkl`: saved trained model.
- `reports/figures/eda`: screenshots from EDA work.
- `reports/figures/ml`: screenshots from ML work.
- `reports/yes_bank_presentation.pptx`: project presentation.
- `README.md`: project summary for GitHub/submission.
- `requirements.txt`: packages required to run the notebooks.

The zip file in Downloads also contains a `yes bank.pptx` presentation. That file is mostly image-based, so the notebooks are the better source for understanding the project.

## Where You Should Start

Start with the dataset, not the model.

1. Open `data/raw/yes_bank_stock_prices.csv`.
2. Understand each column.
3. Open the EDA notebook and run it from top to bottom.
4. Study the charts and write what each chart tells you.
5. Open the ML notebook and run it from top to bottom.
6. Compare Linear Regression, Decision Tree, and Random Forest.
7. Explain why the final model was selected.
8. Prepare your final README, notebook outputs, and PPT.

## How To Run Locally

From the project folder:

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook
```

Then open the notebooks inside the `notebooks` folder and run all cells.

## Your Deadline Plan

Today, July 17, 2026:

- Understand the project objective.
- Run the EDA notebook.
- Learn the meaning of the charts and write notes.

July 18, 2026:

- Run the ML notebook.
- Understand the three models and evaluation metrics.
- Make sure the saved model file is created.

July 19, 2026:

- Finalize README, PPT, and notebook explanations.
- Check that all template answer sections are filled.

July 20, 2026:

- Do final submission check.
- Submit notebooks, dataset, README, model file, and PPT as your mentor expects.

## What You Should Be Able To Explain To Your Mentor

- The data is monthly YES Bank stock price data from Jul-2005 to Nov-2020.
- There are 185 rows and 5 columns.
- There are no missing values and no duplicate rows.
- Open, High, Low, and Close prices are strongly correlated.
- YES Bank stock increased strongly until around 2018 and declined sharply after that.
- The ML task is regression because Close is a continuous numeric value.
- Random Forest was selected as the final model because it handled non-linear patterns and gave strong prediction performance.

## Important Note

Stock prediction is difficult in real life because stock prices are affected by news, market sentiment, economy, company performance, and government policy. This project is for learning the Data Science workflow, not for giving real investment advice.
