# House Price Prediction using Machine Learning

This project predicts house prices using machine learning techniques on the King County housing dataset. It includes data exploration, visualization, feature analysis, and model training using Linear Regression and Gradient Boosting Regressor.

## Files
- `housesales.ipynb` — main notebook containing the full workflow
- `kc_house_data.csv` — dataset used for training and analysis
- `requirements.txt` — project dependencies

## Project Workflow
1. Import libraries and load dataset
2. Perform exploratory data analysis
3. Visualize important features such as bedrooms, location, and living area
4. Train a Linear Regression model
5. Train a Gradient Boosting Regressor
6. Compare model performance

## Models Used
### Linear Regression
Used as a baseline regression model.

**R² Score:** ~0.732

### Gradient Boosting Regressor
Used to capture more complex non-linear relationships in the housing data.

**R² Score:** ~0.919

## Key Insights
- Most houses in the dataset are concentrated around 3–4 bedrooms.
- Features such as square footage and location strongly influence house prices.
- Gradient Boosting performed significantly better than Linear Regression, showing that house prices depend on more complex feature interactions than a simple linear model can capture.

## Issues Resolved During Implementation
While running the notebook, some parts of the original code required updates due to newer library versions:
- Replaced outdated `loss='ls'` with `loss='squared_error'`
- Removed incorrect plotting call `plt1 = plt()`
- Fixed `sns.despine` usage by calling `sns.despine()`
- Adjusted some model input handling using `.values` for compatibility with the current scikit-learn version

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## How to Run
1. Clone the repository
2. Create and activate a virtual environment
3. Install dependencies:
   ```bash
   pip install -r requirements.txt