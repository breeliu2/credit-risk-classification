# Module 12 Report Template

## Overview of the Analysis
The objective of this analysis is to utilize various machine learning techniques to train and assess the performance of Logistic Regression Models in identifying the creditworthiness of borrowers. The models were trained using different methods, and their performances were compared to determine the superior model. The predictive variables in the model correspond to the labels 0 (representing healthy loans) and 1 (indicating high-risk loans).

During the model construction process, the dataset was divided into features and labels, and subsequently split into training and testing sets.

Machine Learning Model 1 was established by creating an instance of the logistic regression model and training it with the original training sets (X_train, y_train). The model was then fitted to the training sets, and predictions were generated.

Machine Learning Model 2 was developed by resampling the original training data using the RandomOverSampler module. Subsequently, a logistic regression model was instantiated and trained with the resampled training sets (X_resample, y_resample). Predictions were generated using this model.

The performance of each model was evaluated based on the balance accuracy score, the confusion matrix, as well as the precision score, recall score, and f1-score as outlined in the classification report. These evaluations were crucial in determining the effectiveness of the models in distinguishing between healthy loans and high-risk loans.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  Model 1, trained on the original data, exhibits an impressive accuracy of 95.2% in predicting the two labels. It excels in accurately predicting healthy loans, with both precision and recall scores reaching and nearing 1.00, signifying a perfect prediction rate.

  However, there is room for improvement in predicting high-risk loans. The precision score for high-risk loans stands at 0.85, indicating that only 87% of the actual high-risk loans were correctly identified by the model. Similarly, the recall score for high-risk loans is 0.89, suggesting that the model identified only 91% of all high-risk loans present in the dataset.

  Enhancing the model's performance in predicting high-risk loans is crucial, and further refinement could lead to more robust and reliable results.



* Machine Learning Model 2:
  * Model 2, trained on the resampled data, achieves an exceptional accuracy of 99.4% in predicting the two labels. The model demonstrates outstanding performance in accurately predicting healthy loans, with both precision and recall scores reaching and nearing a perfect 1.00.

  Regarding high-risk loans, the precision was at 0.84. However, the recall score has significantly improved to 0.99, suggesting that the model is now capable of identifying all high-risk loans present in the dataset.

  The enhanced recall score for high-risk loans is a positive development, highlighting the model's improved ability to capture all relevant instances of high-risk loans, making it more reliable for this critical classification task.






## Summary
The analysis indicates that Model 2 outperforms Model 1 in predicting high-risk loans and demonstrates an overall higher accuracy in predicting both labels. Notably, Model 2 achieved a considerably high precision in identifying high-risk loans, correctly capturing all instances of high-risk loans in the dataset. This level of performance is commendable in this context.

Given these results, I recommend utilizing Model 2 for identifying high-risk loans, as it exhibits superior performance in this crucial task and offers better overall accuracy in predicting the labels. It provides more reliable and precise results, making it the preferred choice for this particular application.
