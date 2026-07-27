# Employee Attrition Prediction using Decision Tree and Random Forest Classification

## Objective

The objective of this assignment is to predict whether an employee is likely to leave an organization based on demographic, professional, and work-related attributes. Two machine learning classification models, Decision Tree and Random Forest, are developed and compared using various evaluation metrics.

## Dataset

The dataset used in this assignment is the IBM HR Analytics Employee Attrition & Performance dataset.

Dataset Link: https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset

The dataset is not included in this repository. It can be downloaded from the provided Kaggle link.

## Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Methodology

The following steps were performed:

1. Loaded the IBM HR Analytics Employee Attrition & Performance dataset using Pandas.
2. Displayed the first five records of the dataset.
3. Identified numerical features, categorical features, and the target variable.
4. Examined the dataset information and summary statistics.
5. Checked the dataset for missing values.
6. Removed unnecessary columns that do not contribute meaningful information to the prediction.
7. Encoded categorical variables using Label Encoding.
8. Separated the input features and target variable.
9. Split the dataset into 80% training data and 20% testing data.
10. Developed a Decision Tree Classifier.
11. Developed a Random Forest Classifier with 100 estimators.
12. Trained both models using the same training dataset.
13. Predicted employee attrition on the test dataset.
14. Evaluated both models using Accuracy, Precision, Recall, and F1-Score.
15. Generated confusion matrices for both models.
16. Generated a feature importance plot for the Random Forest model.
17. Compared the performance of the Decision Tree and Random Forest models.

## Results

The models were evaluated using Accuracy, Precision, Recall, and F1-Score.

| Model | Accuracy | Precision | Recall | F1-Score |
|---|---:|---:|---:|---:|
| Decision Tree | 0.7823 | 0.3191 | 0.3191 | 0.3191 |
| Random Forest | 0.8435 | 0.5455 | 0.1277 | 0.2069 |

## Model Comparison

The Random Forest model achieved higher Accuracy and Precision compared to the Decision Tree model. Its Accuracy was 0.8435 compared to 0.7823 for the Decision Tree, while its Precision was 0.5455 compared to 0.3191.

However, the Decision Tree performed better in terms of Recall and F1-Score. The Decision Tree achieved a Recall of 0.3191 and an F1-Score of 0.3191, while the Random Forest achieved a Recall of 0.1277 and an F1-Score of 0.2069.

For employee attrition prediction, Recall is particularly important because it indicates how effectively the model identifies employees who actually leave the organization. Based on Recall and F1-Score, the Decision Tree performs better in identifying potential employee attrition cases. On the other hand, Random Forest provides better overall Accuracy and Precision.

Random Forest often performs better than a single Decision Tree because it combines the predictions of multiple decision trees, reducing overfitting and making the model more robust. However, in this particular experiment, the Decision Tree achieved better Recall and F1-Score, making it more suitable when identifying potential attrition cases is the primary objective.

## Conclusion

In this assignment, Decision Tree and Random Forest classification models were developed to predict employee attrition using the IBM HR Analytics Employee Attrition & Performance dataset. Both models were trained using the same 80% training and 20% testing split and evaluated using Accuracy, Precision, Recall, and F1-Score. The Random Forest model achieved better Accuracy and Precision, with scores of 0.8435 and 0.5455 respectively. However, the Decision Tree achieved better Recall and F1-Score, with both scores being 0.3191 compared to 0.1277 Recall and 0.2069 F1-Score for Random Forest. Since identifying employees who are likely to leave is important in an attrition prediction problem, Recall and F1-Score are valuable evaluation metrics, making the Decision Tree more suitable for this particular objective. Random Forest often outperforms a single Decision Tree because it combines multiple trees, reducing overfitting and improving robustness. A limitation of Decision Trees is that they can easily overfit the training data. A limitation of Random Forest is that it is more computationally expensive and less interpretable than a single Decision Tree.
