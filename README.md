
# 📊 HR Analytics: Employee Attrition & Performance


## Authors

This project was developed by [Dendi Apriyandi](https://www.linkedin.com/in/dendiapriyandi) and [Clara Putri](https://www.linkedin.com/in/clara-putri-herlin) , an entry level data analyst and data scientist.
## Project Overview

This project focuses on analyzing employee attrition and performance using HR analytics data. The main goal is to help organizations identify key patterns related to employee turnover, predict attrition, and derive actionable insights for better workforce management.

The project consists of three main phases:

    1. Exploratory Data Analysis (EDA): Identifying trends, handling missing data, and visualizing key insights.

    2. Clustering: Grouping employees into meaningful clusters based on performance and behavioral data.

    3. Modeling: Developing predictive models to forecast employee attrition with optimized accuracy.
## Table of Content

1. Project Structure
2. Data Preprocessing & EDA
3. Clustering
4. Model Development
5. Performance Metrics
6. Results & Insights
7. Conclusion
8. Future Improvements
## Project Structure

The project is divided into three notebooks:

- EDA-of-HR-Analytics-Employee-Attrition-&-Performance.ipynb: Contains exploratory data analysis and data cleaning steps.

- Clustering-of-HR-Analytics-Employee-Attrition-&-Performance.ipynb: Implements clustering to uncover meaningful patterns.

- Model-of-HR-Analytics-Employee-Attrition-&-Performance.ipynb: Builds and evaluates machine learning models for predicting employee attrition.
## Data Preprocessing and EDA

In the EDA phase, we clean and analyze the dataset to uncover initial insights:

- Handling missing values: Imputed missing values using appropriate statistical methods.

- Outlier detection and handling: Applied Tukey’s rule to cap extreme values.

- Visualization: Histograms, boxplots, and pairplots were used to explore relationships between features.


Sample visualization from EDA:

- Employee attrition rates are higher among employees with lower job satisfaction.

- Employees with more years in the company tend to stay longer unless job satisfaction is low.
## Clustering

Using K-Means clustering, employees were grouped into distinct clusters based on features such as:

- Job performance

- Years at the company

- Satisfaction level

Clusters provide insights into groups of employees at risk of leaving and high performers who might need additional support or promotion.
## Model Development

Several models were evaluated for predicting employee attrition:

- Baseline Model: Random Forest with default hyperparameters.

    - Achieved perfect metrics on training data (Accuracy: 1.00) but indicated overfitting.

- Optimized Model: Random Forest with hyperparameter tuning to reduce overfitting.

    - Hyperparameters tuned: Number of estimators, max depth, and feature selection.
## Performance Metrics

The following metrics were used to evaluate the models:

- Precision: Measures the proportion of positive identifications that were correct.

- Recall: Measures the ability to find all positive cases.

- Accuracy: The overall proportion of correct predictions.

- F1-Score: The harmonic mean of precision and recall.

Performance Comparison:

| **Metric**     | **Baseline (Test Data)** | **Optimized RF (Test Data)** |
|----------------|--------------------------|------------------------------|
| Precision      | 0.887                    | 0.887                        |
| Recall         | 0.923                    | 0.923                        |
| Accuracy       | 0.836                    | 0.836                        |
| F1-Score       | 0.904                    | 0.904                        |

The optimized Random Forest model reduced overfitting while maintaining comparable performance on the test data.
## Result and Insight

- EDA Findings:

    - Employees with low satisfaction are more likely to leave.
    - Longer tenure reduces attrition risk, unless combined with low job satisfaction.
    

- Clustering Insights:

    - Identified clusters of employees likely to leave, helping the HR team prioritize interventions.

    - High performers were grouped into specific clusters, signaling potential candidates for promotion.

- Model Results:

    - The optimized model successfully mitigated overfitting without compromising accuracy.
    - Recall remained high, ensuring the model accurately captures potential attrition cases.
## Future Improvement

- Explore other algorithms: Trying Gradient Boosting or XGBoost for better predictions.

- Feature engineering: Adding interaction features between variables to improve model performance.

- Deploy the model: Integrate the model into a web app or dashboard for real-time predictions.

- Focus on minority class precision: Optimize precision for minority groups to reduce false positives.