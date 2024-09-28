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

## Project Structure

The project is divided into several key phases, with each phase stored in its respective folder. Below is a breakdown of the tasks included in each step of the project:

### 1. **Project Proposal Tasks**

- **Gathering information**: Notes from the last executive meeting at Automatidata were reviewed to identify the project goals and deliverables.
- **Assigning PACE stages**: Tasks were categorized into the PACE (Planning, Analysis, Construction, Execution) framework to streamline project management.
- **Organizing milestones**: Each task was assigned a milestone to track progress.
- **Creating a project proposal**: A formal proposal was developed for the executive team’s approval, outlining the scope, timeline, and deliverables for the project.

### 2. **Understand the Data Tasks**

- **Loading and exploring the data**: The New York City TLC dataset was loaded into Python, where initial exploration helped identify key variables and data characteristics.
- **Custom functions**: Specific functions were written to clean, organize, and preprocess the dataset, ensuring it was suitable for further analysis.
- **Building a dataframe**: A well-structured dataframe was created to facilitate exploratory data analysis and modeling.
- **Executive summary**: A concise executive summary was produced to provide Automatidata with a clear understanding of the dataset’s structure, quality, and potential insights.

### 3. **Exploratory Data Analysis (EDA) Tasks**

- **Loading and exploring the data**: Reiterating the importance of understanding the dataset, additional exploration was conducted using Python to uncover relationships between variables.
- **Custom functions for EDA**: New functions were developed to visualize data trends, such as the relationship between fare amounts, trip distances, and tipping behavior.
- **Building a dataframe**: The final cleaned dataframe was optimized for further analysis.
- **Executive summary**: An executive summary was created for internal stakeholders, detailing key findings from the EDA, such as correlations and outliers in the data.

### 4. **Statistical Tests Tasks**

- **Descriptive statistics**: Basic statistical metrics were computed to summarize the data, such as mean, median, and standard deviation of taxi tips, trip distances, and fares.
- **Hypothesis testing**: Statistical tests were conducted to examine significant relationships within the dataset, such as whether the trip distance impacts tip amounts.
- **Executive summary**: The results of the statistical tests were summarized for Automatidata’s data team before sharing them with external stakeholders.

### 5. **Regression Modeling Tasks**

- **Descriptive statistics**: Similar to the statistical tests step, basic statistical metrics were calculated to assess the regression model inputs.
- **Regression model**: A linear regression model was developed to predict taxi tips based on features such as fare amount, distance, and payment type.
- **Executive summary**: A summary of the regression model’s performance, including key evaluation metrics such as R-squared and Mean Squared Error (MSE), was provided for Automatidata’s internal review.

### 6. **Machine Learning Models Tasks**

- **Random forest model**: A machine learning model, specifically a random forest, was built to improve prediction accuracy compared to the linear regression model.
- **Executive summary**: A detailed summary of the model’s performance, including feature importance and accuracy metrics, was created for Automatidata’s internal team before the final results were shared with the client.


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
