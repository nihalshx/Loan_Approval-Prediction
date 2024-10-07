# Loan Approval Prediction

This project aims to predict loan approval status based on various financial and personal factors. The dataset used for this project is sourced from Kaggle.

## Dataset

The dataset contains the following features:

- `loan_id`
- `no_of_dependents`
- `education`
- `self_employed`
- `income_annum`
- `loan_amount`
- `loan_term`
- `cibil_score`
- `residential_assets_value`
- `commercial_assets_value`
- `luxury_assets_value`
- `bank_asset_value`
- `loan_status` (target variable)

The target variable `loan_status` indicates whether a loan was approved (`1`) or rejected (`0`).

## Project Structure

1. **Data Loading and Preprocessing**
2. **Encoding Categorical Variables**
3. **Feature Standardization**
4. **Data Splitting**
5. **Model Training and Evaluation**

## Models Used

### Feedforward Neural Network (FNN) or Multilayer Perceptron (MLP)

The Feedforward Neural Network (FNN) model achieved an accuracy of 0.6183 on the test set. This model consists of several dense layers with ReLU activation, batch normalization, and dropout layers to prevent overfitting.

### XGBoost Model

The XGBoost model significantly outperformed the FNN, achieving an accuracy of 0.9883 on the test set. XGBoost is a powerful gradient boosting framework that is particularly effective for structured/tabular data.

## Accuracy Difference

The substantial difference in accuracy between the FNN and XGBoost models can be attributed to the nature of the dataset. XGBoost is highly effective at capturing the relationships in structured data through its boosting mechanism, leading to better performance in this case. Neural networks, on the other hand, are generally better suited for unstructured data such as images or text.

## Key Points

- **Data Preprocessing**: Encoding categorical variables and standardizing features were crucial steps in preparing the data for model training.
- **Model Selection**: Both a neural network and a gradient boosting model were used to evaluate performance. The XGBoost model provided superior accuracy.
- **Model Training**: Proper splitting of the dataset into training, validation, and test sets ensured that the models were evaluated fairly and robustly.
- **Early Stopping**: Used in both models to prevent overfitting and ensure the best performance on the validation set.

## Conclusion

This project demonstrated how to preprocess data, encode categorical variables, standardize features, and train both neural network and gradient boosting models to predict loan approval status. The XGBoost model proved to be significantly more accurate, highlighting the importance of model selection based on the data characteristics.

## References

- Dataset: [Kaggle Loan Approval Dataset](https://www.kaggle.com/datasets/architsharma01/loan-approval-prediction-dataset)
- [TensorFlow Documentation](https://www.tensorflow.org/)
- [XGBoost Documentation](https://xgboost.readthedocs.io/)

