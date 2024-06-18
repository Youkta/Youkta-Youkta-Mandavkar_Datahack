### Predicting Vaccine Acceptance Using Machine Learning

#### Overview
This project focuses on predicting vaccine acceptance (`xyz_vaccine` and `seasonal_vaccine`) using machine learning techniques. It utilizes demographic, behavioral, and attitudinal data to forecast individual vaccination decisions.

#### Approach and Methodology
1. **Data Preprocessing**:
   - Missing values in categorical columns were handled by filling them with 'missing'.
   - Categorical variables were frequency encoded to convert them into numerical features suitable for modeling.

2. **Model Selection and Training**:
   - **CatBoostClassifier** was selected for its robust handling of categorical data.
   - Hyperparameters such as learning rate, depth, and regularization were optimized using grid search.
   - Models were separately trained to predict `xyz_vaccine` and `seasonal_vaccine`.

3. **Evaluation**:
   - Model performance was evaluated using the ROC AUC score to assess predictive accuracy.

4. **Prediction and Submission**:
   - Trained models were used to predict vaccine acceptance on a new dataset (`df2`).
   - Predicted probabilities were compiled into a submission file (`submission.csv`) containing `respondent_id`, `xyz_vaccine`, and `seasonal_vaccine`.

#### Results
- Achieved ROC AUC scores of approximately 0.873 for `xyz_vaccine` and 0.865 for `seasonal_vaccine`, indicating strong predictive performance.

#### Technologies Used
- Python, Pandas, Scikit-learn for data processing and modeling.
- CatBoost for categorical data handling and model training.

#### Conclusion
This project demonstrates the effective use of machine learning to forecast vaccine acceptance based on diverse individual characteristics. It provides insights valuable for public health strategies and decision-making processes.
