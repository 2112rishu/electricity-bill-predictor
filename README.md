# ⚡ Electricity Bill Predictor

## 📌 Project Overview

The **Electricity Bill Predictor** is a machine learning project that predicts daily household electricity consumption using historical electricity usage data. It also estimates the electricity cost based on an assumed price per unit.

The project uses **Linear Regression** to forecast electricity consumption and **Mean Absolute Error (MAE)** to evaluate prediction performance.

## 🎯 Objectives

- Clean and prepare historical electricity consumption data.
- Explore daily electricity usage patterns.
- Analyze average consumption by day of the week.
- Create features for predicting electricity consumption.
- Train and evaluate a machine learning model.
- Predict next-day electricity consumption.
- Estimate a 30-day electricity cost.

## 📊 Dataset

**Dataset:** Individual Household Electric Power Consumption

**Source:** UCI Machine Learning Repository

The dataset contains household electricity measurements collected at approximately one-minute intervals.

Important columns include:

- `Date` — date of the measurement
- `Time` — time of the measurement
- `Global_active_power` — active power consumption in kilowatts
- `Global_reactive_power` — reactive power
- `Voltage` — voltage measurement
- `Global_intensity` — current intensity
- `Sub_metering_1`, `Sub_metering_2`, `Sub_metering_3` — electricity sub-metering measurements

## 🛠️ Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook
- GitHub

## ⚙️ Project Workflow

1. Download and load the dataset.
2. Clean missing and invalid values.
3. Convert date and time columns into a datetime column.
4. Aggregate minute-level readings into daily energy consumption in kWh.
5. Visualize daily consumption and weekday patterns.
6. Create features using previous-day consumption, day of the week, and month.
7. Split the data chronologically into training and testing sets.
8. Train a Linear Regression model.
9. Evaluate performance using MAE.
10. Predict next-day electricity consumption.
11. Estimate the 30-day electricity energy cost.

## 🤖 Machine Learning Model

**Algorithm:** Linear Regression

**Input features:**
- Previous day's electricity consumption
- Day of the week
- Month

**Target variable:** Daily electricity consumption in kWh

**Evaluation metric:** Mean Absolute Error (MAE)

MAE measures the average absolute difference between actual and predicted electricity consumption. A lower MAE indicates smaller prediction errors.

## 📈 Results

The notebook produces:
- Daily electricity consumption graphs
- Average consumption by weekday
- Actual versus predicted consumption plots
- MAE evaluation results
- Next-day consumption predictions
- An estimated 30-day electricity cost

The exact numerical results are available in the executed notebook.

## 💰 Electricity Cost Estimation

The project uses an assumed tariff of **₹8 per kWh** for demonstration.

Estimated 30-day cost:

`Predicted daily consumption × 30 × ₹8`

This is a simplified estimate, not an official electricity bill. Actual bills may include tariff slabs, fixed charges, taxes, and other fees.

## 🚀 How to Run the Project

1. Open the notebook in this repository.
2. Click **Open in Colab**, or download the notebook and upload it to Google Colab.
3. Run the notebook cells in order.
4. Allow the dataset to download.
5. Review the graphs, MAE, prediction, and cost estimate.

Required libraries:

```bash
pip install pandas numpy matplotlib scikit-learn requests
```

## ⚠️ Limitations

- Electricity consumption varies with weather, household activity, and other factors not included in the model.
- The model uses only a small set of features.
- Missing minute-level readings may lead to underestimation of daily energy consumption.
- The monthly cost estimate assumes the predicted daily consumption stays constant for 30 days.
- The assumed tariff may differ from the actual electricity tariff.

## 🔮 Future Improvements

- Compare Linear Regression with Random Forest and other forecasting models.
- Add weather and holiday information.
- Include more historical consumption features.
- Improve handling of missing readings.
- Use actual electricity tariff slabs for more realistic bill estimates.
- Deploy the model as a simple web application.

## 👨‍💻 Author

**Name:** [Akshat]

## 📄 License

This project is intended for educational and learning purposes.
