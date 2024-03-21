## Time Series Energy Consumption Forecasting with XGBoost

## Overview:
This project aims to forecast energy consumption using historical hourly data of energy usage (PJME - AEP Hourly Time Series Data). The forecasting model is built using XGBoost, a popular gradient boosting algorithm known for its performance and efficiency.

## Files Included:
- `PJME_hourly.csv`: The dataset containing hourly energy consumption data.
- `energy_prediction.ipynb`: Jupyter Notebook file containing the Python code for data preprocessing, feature engineering, model training, and prediction.
- `README.md`: This file, providing an overview of the project and instructions for running the code.

## Dependencies:
- Python 3.x
- Libraries: pandas, numpy, matplotlib, seaborn, xgboost, sklearn

## Setup Instructions:
1. Clone the repository to your local machine.
2. Install the required dependencies using pip:
3. Open the Jupyter Notebook `energy_consumption_forecasting.ipynb` using Jupyter Notebook or JupyterLab.
4. Run each cell in the notebook sequentially to execute the code and reproduce the analysis.

## Project Structure:
1. **Data Preprocessing**: 
- Loading the dataset
- Handling missing values
- Removing outliers

2. **Time Series Cross-Validation**:
- Splitting the data using TimeSeriesSplit
- Visualizing the train-test splits

3. **Feature Engineering**:
- Creating features such as hour, day of week, quarter, etc.
- Adding lag features to capture historical trends

4. **Model Training**:
- Training an XGBoost regressor model
- Using TimeSeriesSplit for cross-validation

5. **Future Prediction**:
- Training the model on the entire dataset
- Generating future dates for prediction
- Predicting future energy consumption using the trained model

## Results:
- The model achieves a root mean squared error (RMSE) of approximately 3746.85 across the five folds of cross-validation.
- Future predictions are made for energy consumption for the next one year.

## References:
- [PJME - AEP Hourly Time Series Data](https://www.kaggle.com/robikscube/hourly-energy-consumption):This data represents the estimated energy consumption in megawatts (MW) for the PJM East Region for the years 2001 to 2018
It can be used  to analyze energy consumption trends, seasonal variations, and other patterns that might be present in the electricity consumption of the PJM East Region over those years. This kind of analysis can provide valuable insights into energy demand and help with planning and decision-making in the energy sector.
- [XGBoost Documentation](https://xgboost.readthedocs.io/)
- [scikit-learn Documentation](https://scikit-learn.org/stable/documentation.html)

