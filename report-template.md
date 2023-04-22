# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).


Credit-risk analysis predicts the risk level ("healthy_loan" and "high_risk") associated with loans based on the features from the dataset. The information used for this analysis is from past lending activity of the clients which includes loan size, interest rate, debt-to-income ratio, number of accounts and derogratory marks. These are the independent variable (X) used in performing the predictive model. The dependent variable (y) is the loan status to classify if it's "healthy_loan" and "high_risk".

The stages of the machine learning process of this analysis: firstly, split the data using subset information for training and testing model. Secondly, train the large subset of data to teach the model in recognising classification pattern. Then, validate the data using a small subset to test how well the model is able to predict labels. Lastly, use the logisitic regression model to predict labels for unclassified data.



## Results

* Machine Learning Model 1:

![Model_original](https://user-images.githubusercontent.com/117326039/233763937-0bdeb49d-cd74-4397-906b-8684a1a35a5a.png)

<br>
<br>

* Machine Learning Model 2:

![Model_oversampled](https://user-images.githubusercontent.com/117326039/233763996-99c89de9-2fcf-4e94-a227-0df56c3def1a.png)

 
## Summary

Summarise the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.



This credit-risk analysis demonstrates the importance of considering imbalanced data and utilizing appropriate techniques to address it. It also highlights the importance of evaluating the performance of the model using various metrics to ensure that it is performing well for both classes.

Both logistic regression models for original and oversampled dataset have high accuracy result. However, on the oversampled data, it outperformed the one trained on the original dataset in terms of precision, recall, and F1-score for "high_risk" loans. This means that this model performs well for both "healthy_loan" and "high_risk".

The performance of the model does depend on the problem wfor this credit-risk analysis. In this case, it is more important to predict the "high_risk" loans accurately because they are the ones that may result in financial losses. The logistic regression model trained on the oversampled data performs well in this regard with high precision and recall values for "high_risk" loans.
