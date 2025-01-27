# Telcom-Customer-churn-predictor

This project focuses on predicting customer churn using a Random Forest Classifier. The dataset contains customer activity details such as call information, account details, and churn status. The objective is to identify key factors influencing churn and build a model to improve customer retention strategies.

## Project Overview

- **Goal:** Develop a predictive model to identify customers likely to churn.
- **Dataset:** Customer activity data, including features like call details and account information. The dataset is split into an 80% training/validation set and a 20% testing set.
- **Key Insights:** Features such as `Total day charge`, `Customer service calls`, and `International plan` significantly impact churn prediction.

## Approach

1. **Data Preprocessing:**
   - Encoded categorical variables.
   - Treated outliers using the Interquartile Range (IQR) method.
   - Balanced class imbalance with SMOTE (Synthetic Minority Oversampling Technique).
   - Standardized numerical features using `StandardScaler`.

2. **Exploratory Data Analysis (EDA):**
   - Identified correlations between features and the target variable.
   - Visualized distributions and outliers with histograms and boxplots.

3. **Model Selection and Training:**
   - Chose a Random Forest Classifier for its ability to handle non-linear relationships and interpret feature importance.
   - Trained the model on resampled data using SMOTE to address class imbalance.

4. **Evaluation:**
   - Used metrics like accuracy, precision, recall, F1-score, and confusion matrix to assess performance.
   - Achieved a test accuracy of **95.6%**, with a recall of **71.5%** for the churn class.

## Results

- **Validation Accuracy:** 94.5%
- **Test Accuracy:** 95.6%
- **Key Metrics:**
  - **Precision (Churn):** 0.971
  - **Recall (Churn):** 0.715
  - **F1-Score (Churn):** 0.824

## Technologies Used

- **Python Libraries:**
  - `Pandas` and `NumPy`: Data manipulation and preprocessing.
  - `Matplotlib` and `Seaborn`: Visualization.
  - `Scikit-learn`: Model training, evaluation, and preprocessing.
  - `Imbalanced-learn`: SMOTE for handling class imbalance.

## Project Structure

- **Code:** Refer to the attached notebook `Final_Customer_Churn_project.ipynb` for the complete implementation.
- **Dataset:** The churn dataset, split into training and testing sets, is used for modeling.

## Conclusion

The project demonstrates the successful application of a Random Forest Classifier for churn prediction. By addressing data imbalance with SMOTE and optimizing features, the model achieved high accuracy and balanced recall. Insights from the analysis can help businesses develop targeted customer retention strategies.

