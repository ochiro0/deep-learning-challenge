# deep-learning-challenge


## Introduction
Alphabet Soup, a nonprofit foundation, aims to select the best applicants for funding with the highest chance of success in their ventures. To achieve this, we have utilized machine learning and neural networks to build a binary classifier that predicts whether applicants will be successful if funded by Alphabet Soup.

## Findings

### Data Preprocessing

* The target variable for our model is the 'IS_SUCCESSFUL' column from the 'application_df' dataset, indicating whether the funding was used effectively.
* The feature variables used for prediction include: AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT.
* The 'EIN' and 'NAME' columns, serving as identification, were removed as they have no direct impact on the target variable or act as features.

### Model Compilation, Training, and Evaluation

* Our initial neural network model had a two-layer architecture with specific choices for neurons, layers, and activation functions.
* The first hidden layer had 80 neurons with ReLU activation, the second hidden layer had 30 neurons with ReLU activation, and the output layer had one neuron with a sigmoid activation for binary classification.
* However, the achieved model accuracy was 73%, falling short of the target performance of 75%.

### Attempts to Increase Model Performance

* Increasing the number of neurons and epochs: This approach didn't improve the accuracy beyond 73%, and it also posed the risk of overfitting.
* Adding more layers to the model: Although this can enhance the model's capacity to learn complex relationships, it also didn't result in improved accuracy.
* Using a different activation function (tanh for the second layer): Introducing tanh activation didn't lead to an accuracy boost.
* Utilizing an Automated Optimiser: Employing hyperparameter tuning didn't yield better results either.

## Conclusion
* The developed deep learning model fell short of the target accuracy, achieving only 73%. To enhance the model's performance, several strategies can be considered:

1. Adding more data: Increasing the size of the training dataset can improve generalization capability and accuracy. Collecting more relevant data can provide valuable insights for better predictions.
2. Checking data cleaning: Ensuring proper data cleaning, handling missing values, outliers, and addressing data quality issues can improve model performance.
3. Exploring alternative algorithms: Trying different algorithms, such as Random Forest, can identify key predictor columns and potentially improve accuracy.
4. Identifying feature importance and selecting relevant attributes: Analyzing feature importance helps focus on informative features, reducing noise, and improving accuracy.
Addressing high bias and outliers: Identifying and handling outliers can mitigate their impact on model performance.
5. Binning the data: Binning continuous variables can simplify the relationship between variables and the target, making the model more robust.

* In summary, optimizing the deep learning model requires iteratively experimenting with various strategies and evaluating their impact on model performance. Fine-tuning the model and considering different approaches can lead to improved accuracy and better predictions for Alphabet Soup's funding selection process.

