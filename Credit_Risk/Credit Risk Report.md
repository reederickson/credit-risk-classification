# Module 12 Report Template

## Overview of the Analysis

The purpose of this analysis is to evaluate the performance of a machine learning model trained to predict loan statuses as either "healthy loan" (0) or "high-risk loan" (1). The model is crucial for assisting the peer-to-peer lending services company in identifying risky loans early on, thereby mitigating potential losses and optimizing their lending practices. The dataset contained information on various attributes of loans, such as credit score, income loan amount, and loan status. The objective was to predict whether a loan is deemed "healthy" or "high-risk" based on the provided financial information. The variables to predict included loan statuses, with the following distribution: "healthy_loan": 18765 instances, "high_risk_loan": 619 instances.

#### Stages of Machine Learning Process
The machine learning process involved several stages:
**Data Processing**: the dataset was cleaned and preprocessed to handle categorical variables, missing values, and feature scaling.
**Feature Selection**: Relevant features were selected to train the model, considering their importance in predicting loan status. For this model, the relevant feature was "loan status"
**Model Training**: Various machine learning algorithms were trained on the preprocessed data to learn patterns and relationships between features and loan statuses
**Model Evaluation**: the trained models were evaluated using performance metrics such as accuracy, precision, and recall to assess their effectiveness in predicting loan statuses.

#### Methods Used
During the analysis, logistic regression was utilized as one of the algorithms to train the machine learning model. The model's performance was evaluated by generating a confusion matrix and going over its classification report.


## Results

The performance metrics of the machine learning model are as follows:

- Accuracy measures the proportion of correctly classified instances out of the total instances in the dataset. It is calculated as the ratio of the number of correct predictions to the total number of predictions. The closer the accuracy score is to 1, the higher the accuracy of the model.
* **Accuracy Score**: 0.99


- Precision measures the accuracy of positive predictions
* **Precision Score**:
"healthy_loan": 1.00
"high_risk_loan": 0.85


- Recall measures the proportion of actual positives that were correctly identified
* **Recall Scor**e:
"healthy_loan": 0.99
"high_risk_loan": 0.91


## Summary
The machine learning model exhibits exceptional performance with high accuracy, precision, and recall scores. It effectively predicts loan statuses and accurately identifies high-risk loans. I recommend deploying this model for use by the company, as it would greatly assist in optimizing lending decisions and minimizing potential losses.
#### Performance Evaluation
The accuracy score of 0.99 indicates that the model correctly classifies approximately 99% of the instances in the dataset. The precision score for "healthy_loan" is perfect at 1.00, meaning that when the model predicts a loan as healthy, it is almost always correct. The precision score for "high_risk_loan" is slightly lower at 0.85, indicating that there are some false positives where the model incorrectly predicts a loan as high-risk when it's healthy. Both recall scores are high, suggesting that the model effectively captures the majority of actual instances of both "healthy loan" and "high-risk loan".
#### Recommendation
The choice of the model to use depends on the specific goals and priorities of the peer-to-peer lending services company. If the primary concern is to minimize losses by accurately identifying high-risk loans, then maximizing precision for "high-risk loan" may be crucial. In this case, the model's slightly lower precision for "high-risk loan" might be a concern. However, if overall accuracy and balance between precision and recall for both classes are considered important, then the current model is recommended for deployment.

In summary, while the model exhibits outstanding performance, the choice of the "best" model depends on the specific priorities and trade-offs of the company. If the company prioritizes overall accuracy and balance between precision and recall for both classes, the current model is suitable for deployment. However, if minimizing losses from misclassified high-risk loans is of greatest importance, further optimization or consideration of alternative models may be warranted.