# Income Classification with XGBoost

## Project Overview

This project focuses on predicting whether an individual earns more than $50,000 per year using demographic and employment-related features. The goal is to compare multiple classification models, select the best-performing approach, and interpret how different features contribute to higher income levels.

The analysis follows a standard data science workflow including preprocessing, model training, cross-validation, evaluation on a held-out test set, and model interpretation.

---

## Data

The dataset contains individual-level information such as age, education, occupation, capital gains, and work characteristics. The target variable is a binary indicator of whether income exceeds $50,000 per year.

Key challenges include class imbalance and capturing nonlinear relationships between predictors and income.

--- 

## Modeling Approach

Seven classification models were trained and evaluated using five-fold cross-validation. Performance was assessed using metrics such as accuracy, precision, recall, and F1-score, with particular attention paid to the positive class (income over $50,000).

Based on cross-validation results, XGBoost was selected as the final model due to its strong and consistent performance.

--- 

## Results

On the held-out test set, the final XGBoost model achieved:
	•	Accuracy: 87%
	•	Precision (>$50K): 0.76
	•	Recall (>$50K): 0.68

The model performs especially well given the class imbalance and the difficulty of identifying higher-income individuals. Feature-based analysis highlights the importance of variables such as education, age, and capital gains in predicting income level.

Key Takeaways
	•	XGBoost outperformed other models in cross-validation and test performance.
	•	The model balances predictive performance with interpretability.
	•	Socioeconomic features show clear and meaningful relationships with income outcomes.
