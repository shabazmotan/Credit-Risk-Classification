# Credit Risk Analysis

# Overview of the Analysis

The objective of this analysis is to assess the effectiveness of two logistic regression machine learning models in forecasting the credit risk associated with loans. The analysis was performed on financial data, with a specific emphasis on loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. The goal was to predict the loan's status, distinguishing between a healthy loan (0) and a high-risk loan (1).

The machine learning process in this analysis encompassed the following stages:

1. Dividing the data into separate training and testing datasets.
2. Constructing and training a logistic regression model using the original data.
3. Assessing the model's performance through accuracy, precision, and recall scores.
4. Addressing class imbalance by resampling the data using RandomOverSampler.
5. Constructing and training another logistic regression model using the resampled data.
6. Evaluating the performance of the resampled model using the same metrics.

The methods employed in this analysis involved the utilization of LogisticRegression for constructing the models and RandomOverSampler for resampling the data.

# Results

# Model 1: Logistic Regression with Original
Model 1's Accuracy, Precision, and Recall scores can be described as follows:

Accuracy: The model achieves an overall accuracy of 0.99, indicating that it correctly classifies 99% of instances.

Precision:
 * Healthy loans (0): The model exhibits a precision of 1.00, demonstrating its exceptional ability to correctly identify true positives with minimal false positives.

 * High-risk loans (1): The model shows a precision of 0.87, indicating a moderate effectiveness in identifying high-risk loans with some occurrences of false positives.

Recall:
 * Healthy loans (0): The model attains a recall of 1.00, signifying that it accurately identifies nearly all instances of healthy loans with very few false negatives.

 * High-risk loans (1): The model achieves a recall of 0.89, indicating its effectiveness in identifying high-risk loans while having a few occurrences of false negatives.

# Model 2: Logistic Regression with Resampled Data
Model 2's Accuracy, Precision, and Recall scores can be descibed as follows:

Accuracy: The model achieves an overall accuracy of 0.99, indicating that it correctly classifies 99% of instances.

Precision:
 * Healthy loans (0): The model demonstrates a precision of 0.99, showcasing its excellent ability to accurately identify true positives with minimal false positives.

 * High-risk loans (1): Similarly, the model achieves a precision of 0.99, indicating its effectiveness in correctly identifying high-risk loans with very few false positives.

Recall:
 * Healthy loans (0): The model attains a recall of 0.99, suggesting that it correctly identifies nearly all instances of healthy loans with very few false negatives.

 * High-risk loans (1): The model also achieves a recall of 0.99, indicating its effectiveness in correctly identifying high-risk loans with very few false negatives.

# Summary
Based on the findings, the logistic regression model trained with resampled data (Model 2) outperforms the model trained with original data (Model 1), especially in the prediction of high-risk loans. Model 2 demonstrates higher precision and recall scores for high-risk loans, which is crucial for minimizing potential financial losses for the lending company.

I strongly recommend utilizing the logistic regression model trained with resampled data (Model 2) for credit risk analysis. This model showcases a significant improvement in predicting high-risk loans compared to the original model. By incorporating this model into the loan assessment process, the company can make informed decisions when approving or rejecting loans, thereby effectively mitigating credit risk.