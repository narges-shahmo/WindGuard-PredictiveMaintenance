# WindGuard: Predictive Maintenance for Wind Turbines

## Overview

WindGuard is a predictive maintenance solution designed to forecast failures in wind turbine generators, developed with the goal of reducing operational costs and enhancing the efficiency of wind energy production. Utilizing machine learning techniques, this project analyzes sensor data from wind turbine generators to predict potential failures before they occur, allowing for timely maintenance and repair.

## Project Objectives

- To analyze sensor data from wind turbine generators for signs of impending failure.
- To build and tune various classification models to accurately predict generator failures.
- To select the best-performing model based on recall, precision, and overall cost-effectiveness.

## Data Insights

The project dataset consists of 40,000 observations across 41 sensor readings, with the target variable indicating generator failure (1) or no failure (0). The data preprocessing steps included handling missing values, addressing outliers, and normalizing the distribution of the sensor readings.

## Exploratory Data Analysis (EDA) Highlights

- Sensor readings exhibit a normal distribution with a few outliers, which were appropriately handled.
- Box plots and distribution graphs were used to visualize the data and identify any anomalies.

## Model Development and Performance

Several classification models were developed using original, oversampled, and undersampled datasets to address class imbalance. The models tested include logistic regression, decision trees, random forest, bagging classifier, and boosting methods. After comparing the performance of these models on validation data, XGBoost Classifier, Random Forest on Oversampled data, and XGBoost Classifier on Oversampled data were selected for further tuning.

## Model Selection and Tuning

The XGBoost Classifier model was ultimately selected for its superior performance on both validation and training data. The model demonstrated a balanced trade-off between recall and precision and minimized the operational and maintenance costs associated with predictive maintenance.

## Key Findings and Business Insights

- The model can accurately identify potential failures in wind turbine generators, allowing for preventive maintenance and cost reduction.
- Important predictors of maintenance requirements include sensor readings V18, V39, V3, V26, and V10.
- The predictive model achieved a notable performance on test data, with a significant percentage of true positives and a low rate of false negatives and false positives.
- The project underscores the importance of predictive maintenance in the renewable energy sector and provides a blueprint for operational efficiency.

## Conclusion

WindGuard represents a significant advancement in the predictive maintenance of wind turbines. By leveraging machine learning, ReneWind can anticipate generator failures, optimize maintenance schedules, and ultimately reduce the environmental impact of energy production. The project offers a scalable solution to enhance the reliability and efficiency of wind energy generation.

*Note: This project is part of the coursework from University of Austin's post graduate program.*