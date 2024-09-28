# Predicting Taxi Tips in NYC

## Project Overview

The goal of this project was to build multiple models, including a **multiple linear regression** and a **random forest model**, to predict whether a taxi rider would leave a high gratuity (>20%) or not (<20%). The project utilized data from **yellow taxi trips taken in New York City during 2017**. After rigorous data exploration and model building, the **final random forest model achieved 86% accuracy and 72% precision** in predicting generous tippers. Key factors influencing tipping behavior included the **duration, distance, and cost of the trip**, which were found to be the most important features in distinguishing high tippers from low tippers.

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

**Random Forest Model**: A random forest model consisting of **100 decision trees** was used to improve prediction accuracy by capturing non-linear relationships between the features. The random forest model also provided insights into which features were most important for the prediction task.

### Feature Importance and Data Insights

The dataset, provided by the New York City Taxi & Limousine Commission, contains various features related to taxi trips in NYC during 2017. Key features and their relevance to tipping behavior include:

- **Trip Duration (tpep_pickup_datetime, tpep_dropoff_datetime)**: Longer trip durations often result in higher gratuities.
- **Trip Distance (Trip_distance)**: The distance of the trip impacts the fare and, consequently, tipping behavior.
- **Fare Amount (Fare_amount)**: The metered fare is directly related to the tip amount, with higher fares generally leading to higher tips.
- **Payment Type (Payment_type)**: Riders paying by credit card typically leave tips that are automatically recorded, unlike cash transactions.
- **Vendor ID (VendorID)**: This feature captured differences between the service providers (Creative Mobile Technologies and VeriFone Inc.), which surprisingly emerged as a significant factor.

### Performance of the Random Forest Model

The random forest model was evaluated based on its ability to predict generous tips (>20%) vs. non-generous tips (<20%). The key features driving the predictions were **trip duration**, **trip distance**, and **fare amount**, along with **Vendor ID**. The model achieved the following performance metrics:

#### Random Forest (Cross-Validation):
- **Precision**: 0.675
- **Recall**: 0.757
- **F1 Score**: 0.714
- **Accuracy**: 0.680

#### Random Forest (Test Set):
- **Precision**: 0.675
- **Recall**: 0.779
- **F1 Score**: 0.723
- **Accuracy**: 0.687

### Feature Importance Plot

The following plot displays the top 15 most important features, ranked by their **mean decrease in impurity**, which indicates how much each feature contributed to the model’s ability to classify generous tippers.

![Feature Importances](./feature_importances.png)

The plot highlights that **trip duration, distance, fare amount**, and **Vendor ID** were the most important factors influencing tipping behavior.


## Conclusion

Based on the analysis and modeling, the project delivers a working prediction model that can be integrated into an application to estimate taxi tips in real-time. The random forest model outperformed the linear regression model in terms of accuracy. Future improvements could involve incorporating additional features such as weather conditions or traffic patterns to further enhance tip prediction accuracy.
