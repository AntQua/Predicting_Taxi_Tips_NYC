# Predicting Taxi Tips in NYC

## Project Overview

This project aims to predict the amount of tips given by passengers to taxi drivers in New York City. The project uses data from the New York City Taxi and Limousine Commission (TLC), which oversees taxi services in the city. By building machine learning models, we can provide better insights into the factors influencing tipping behavior, enabling taxi drivers and service platforms to offer enhanced services to their customers. The project utilizes data exploration, regression modeling, and machine learning techniques to achieve accurate predictions.

## Business Understanding

The New York City Taxi and Limousine Commission (TLC) regulates taxi services in NYC, ensuring fair and reliable transportation. TLC aims to improve rider satisfaction by developing an app that estimates fare and tips, which helps manage rider expectations and promote better service. In this context, Automatidata has been tasked to build predictive models that estimate taxi tips, providing an opportunity to increase transparency and efficiency in the service.

## Data Understanding

The data used in this project was sourced from the New York City TLC dataset, which contains detailed information about trips made by taxis in NYC, including pick-up/drop-off locations, trip distances, total fares, and tips. The data covers a broad timeframe, and some key characteristics include:

- Number of Records: 22669 rows– each row represents a different trip
- Features: Distance, Fare, Payment Type, etc.
- Timeframe: 2017.
- Data Limitations: The dataset may include missing or erroneous values, particularly related to payment types and tips, which require cleaning and preprocessing.

Key visualizations from the exploratory data analysis (EDA) are also included in the project to highlight relationships between key features and tipping behavior.

## Modeling and Evaluation

This project employs various statistical and machine learning techniques, including:

1. **Descriptive Statistics:** Basic statistical analysis to understand the data distribution.
2. **Regression Model:** A linear regression model is used to predict taxi tips based on factors such as fare amount, trip distance, and passenger count.
3. **Random Forest Model:** A more advanced machine learning model, random forest, is used to further improve the accuracy of predictions.

The evaluation metrics for the models include:

- **R-squared (R²):** Measures the proportion of variance explained by the model.
- **Mean Squared Error (MSE):** Provides a measure of the model’s prediction error.

## Conclusion

Based on the analysis and modeling, the project delivers a working prediction model that can be integrated into an application to estimate taxi tips in real-time. The random forest model outperformed the linear regression model in terms of accuracy. Future improvements could involve incorporating additional features such as weather conditions or traffic patterns to further enhance tip prediction accuracy.
