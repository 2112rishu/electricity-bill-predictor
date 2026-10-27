# Electricity Bill Predictor

## Project Overview
This project uses machine learning to predict daily household electricity consumption and estimate electricity costs using historical usage data.

## Objectives
- Clean and explore electricity usage data.
- Analyze daily consumption patterns.
- Predict electricity consumption using Linear Regression.
- Estimate electricity costs.

## Dataset
Individual Household Electric Power Consumption dataset from the UCI Machine Learning Repository. The original text data was converted to CSV and processed using Python.

## Technologies Used
- Python
- pandas
- NumPy
- Matplotlib
- scikit-learn
- Google Colab

## Features
- Previous day's electricity consumption
- Day of the week
- Month of the year

## Model and Results
**Model:** Linear Regression

| Metric | Result |
|---|---:|
| Training records | 1,145 |
| Testing records | 287 |
| Mean Absolute Error (MAE) | 4.956 kWh |
| Latest daily usage | 24.80 kWh |
| Predicted next-day usage | 27.08 kWh |

## Estimated Electricity Cost
Using an assumed tariff of ₹8 per kWh, the estimated 30-day energy cost is **₹6,498.10**.

This is a simplified estimate, not an actual electricity bill. It assumes daily consumption remains constant and excludes fixed charges, taxes, and tariff slabs.

## How to Run
1. Open `Electricity_Bill_Predictor.ipynb`.
2. Open the notebook in Google Colab.
3. Run the cells in order.
4. Review the graphs, model evaluation, and predictions.

## Limitations
- Missing readings may affect daily consumption estimates.
- The model uses a limited number of features.
- Actual electricity bills depend on the applicable tariff and other charges.

## Conclusion
This project demonstrates data cleaning, visualization, feature engineering, machine learning, model evaluation, and electricity cost estimation using Python.
