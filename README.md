# Real Estate Price Prediction — Machine Learning

A university machine learning project exploring how property characteristics relate to real estate prices, using exploratory data analysis, regression models, and interactive visualisations.
## Try the Interactive Notebook

Run the notebook in Google Colab to explore the interactive visualisations and real-estate price prediction sliders.

[**Open the Real Estate ML Project in Google Colab →**](https://colab.research.google.com/drive/1D6vat5W3s7LMCAzaO115NqgrDDRAEQbU?usp=sharing)

Run the notebook cells in order and upload the Excel dataset when prompted.
## Project Overview

This project uses the **Real Estate Valuation dataset** from the UCI Machine Learning Repository. It contains 414 real estate transactions in Sindian District, New Taipei City, Taiwan, recorded between August 2012 and July 2013.

The objective is to explore relationships between property prices and features such as house age, distance to the nearest MRT station, number of convenience stores, and geographical location, then compare different regression models.

## Project Workflow

- **Data exploration:** Inspected the dataset structure, descriptive statistics, and potential outliers.
- **Exploratory Data Analysis (EDA):** Created histograms, boxplots, scatterplots, correlation analysis, and geographical visualisations.
- **Data preparation:** Prepared features and target variables and separated the data into training and test sets.
- **Model development:** Trained Linear Regression, Ridge Regression, and Decision Tree Regression models.
- **Model optimisation:** Used cross-validation and hyperparameter tuning to improve model performance.
- **Evaluation:** Compared models using Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R².
- **Interactive exploration:** Built interactive visualisations to investigate relationships between property characteristics and prices.
- **Prediction interface:** Created an interactive interface to estimate unit-area prices using the optimised Decision Tree model.

## Model Performance

The following results were obtained on the held-out test set.

| Model | MAE | RMSE | R² |
|---|---:|---:|---:|
| Linear Regression | 5.305 | 7.315 | 0.681 |
| Optimised Ridge Regression | 5.305 | 7.315 | 0.681 |
| Optimised Decision Tree | **4.727** | **6.457** | **0.751** |

The optimised Decision Tree achieved the lowest prediction errors and the highest R² among the three models evaluated.

The target variable is measured in units of 10,000 New Taiwan dollars per ping. Therefore, MAE and RMSE are expressed in that same unit, not in individual New Taiwan dollars or per square metre.

## Key Learnings

Through this project, I gained practical experience in:

- Exploring and interpreting real-world datasets.
- Identifying patterns, correlations, and potential outliers.
- Applying regression algorithms and comparing their performance.
- Using cross-validation and hyperparameter tuning.
- Interpreting evaluation metrics and residual plots.
- Building interactive visualisations and a simple prediction interface.

This project helped me connect statistical concepts with practical machine learning workflows and understand how model evaluation informs model selection.

## Tools & Technologies

- Python
- Pandas and NumPy
- Matplotlib and Plotly
- Scikit-learn
- Jupyter Notebook / Google Colab
- IPywidgets

## Dataset

**Source:** [UCI Machine Learning Repository — Real Estate Valuation Data Set](https://archive.ics.uci.edu/dataset/477/real+estate+valuation+data+set)

The dataset includes property-related features and unit-area real estate prices. Please refer to the original source for dataset documentation and usage terms.

## How to Run

1. Download or clone this repository.
2. Open the notebook in Google Colab or Jupyter Notebook.
3. Upload `Real estate valuation data set.xlsx` when prompted, if it is not already available in the notebook environment.
4. Run the notebook cells in order.

Some interactive components are designed for notebook environments that support IPywidgets.

## Limitations & Future Improvements

- The dataset is relatively small, with 414 observations, and represents a specific location and historical period.
- Model performance on this dataset does not establish how well the models would predict current prices in other property markets.
- Further work could include stronger validation, additional model comparisons, and a more robust, reusable prediction application.

## Project Context

This is an academic learning project. Its purpose is to demonstrate the application of data analysis and machine learning techniques, rather than provide reliable real-world property valuations.
