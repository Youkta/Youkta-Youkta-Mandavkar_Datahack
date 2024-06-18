### Predicting Vaccine Uptake: A Multi-Label Classification Approach

#### Project Description:
This project aims to predict the likelihood of individuals receiving the xyz flu vaccine and the seasonal flu vaccine using demographic, behavioral, and opinion-related features. The prediction is treated as a multi-label classification problem.

#### Approach:
1. **Data Preprocessing:**
   - Load and merge training features and labels.
   - Handle missing values with `SimpleImputer`.
   - One-hot encode categorical variables and standardize numerical features.

2. **Model Development:**
   - Split the dataset into training and validation sets.
   - Train a `RandomForestClassifier` on preprocessed data.
   - Evaluate using ROC AUC scores for both target variables.

3. **Prediction:**
   - Apply the trained model to the test set.
   - Prepare and save the submission file.

#### Methods and Libraries:
- **Libraries:** `pandas`, `scikit-learn`
- **Data Preprocessing:** `SimpleImputer`, `OneHotEncoder`, `StandardScaler`, `ColumnTransformer`, `Pipeline`
- **Model Training:** `RandomForestClassifier`
- **Evaluation:** `roc_auc_score`

This project employs a structured approach to predict vaccine uptake using machine learning, ensuring accurate model evaluation and effective predictions.
