# Forecasting-Renewable-Energy-Trends-in-the-USA-AI-Driven-Analysis-of-Electricity-Production-25301
## Project Overview

This project focuses on leveraging machine learning techniques to predict electricity production across various energy sources in the USA. The goal is to develop accurate models to forecast energy production trends, enabling better decision-making for energy providers, policymakers, and sustainability advocates.

Three machine learning models were explored: **Support Vector Machine (SVM)**, **Gradient Boosting Classifier**, and **Random Forest Classifier**. Each model underwent hyperparameter tuning to optimize performance.

## Dataset

The dataset comprises electricity production data across diverse energy sources, including Solar, Wind, Nuclear, Bioenergy, Coal, Gas, Hydro, Oil, and Other Renewables. Key features represent conditions influencing energy production, while the target variable is the energy source.

### Business Impact

- **Predictive Insights:** Accurate forecasting aids in optimizing energy production, balancing supply and demand, and reducing energy wastage.
- **Sustainability:** Supports the transition to renewable energy by identifying trends and helping prioritize cleaner energy sources.
- **Operational Efficiency:** Energy providers can make data-driven decisions to optimize infrastructure, improving resilience and cost efficiency.
- **Policy Guidance:** Informs regulatory bodies about energy trends to guide policy frameworks toward sustainable energy.

## Methodology

1. **Data Preprocessing:** Cleaned the dataset and prepared feature-target splits.
2. **Model Selection:** Three models were tested, each optimized using hyperparameter tuning:
   - **SVM:** Randomized Search CV with parameters `C`, `kernel`, and `gamma`.
   - **Gradient Boosting:** Randomized Search CV with parameters `n_estimators`, `learning_rate`, and `max_depth`.
   - **Random Forest:** Grid Search CV with parameters `n_estimators`, `max_depth`, `min_samples_split`, `min_samples_leaf`, and `bootstrap`.
3. **Evaluation:** Accuracy, precision, recall, and F1-score were used as metrics.

## Results

### 1. Support Vector Machine (SVM)
- **Best Parameters:** `{'kernel': 'rbf', 'gamma': 'auto', 'C': 10}`
- **Accuracy:** `95.52%`
- **Insights:** SVM performed well but struggled slightly with imbalanced classes like Wind and Bioenergy.

### 2. Gradient Boosting Classifier
- **Best Parameters:** `{'n_estimators': 100, 'learning_rate': 0.1, 'max_depth': 5, 'min_samples_split': 2, 'min_samples_leaf': 1}`
- **Accuracy:** `97.70%`
- **Insights:** Gradient Boosting showed significant improvements, especially in classifying Solar and Hydro energy with near-perfect scores.

### 3. Random Forest Classifier
- **Best Parameters:** `{'n_estimators': 300, 'max_depth': 30, 'min_samples_split': 2, 'min_samples_leaf': 1, 'bootstrap': True}`
- **Accuracy:** `98.12%`
- **Insights:** Random Forest outperformed all other models, delivering the highest accuracy and excelling in capturing subtle patterns in diverse energy sources.

## Conclusion

- The **Random Forest Classifier** achieved the best performance with an accuracy of **98.12%**, making it the most reliable model for predicting energy production.
- The high performance across models highlights the potential of AI-driven forecasting in energy management, paving the way for optimized resource allocation and a sustainable energy future.


