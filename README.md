---
For this project, I worked with a teammate to build a model to classify the probability an individual's income met a certain threshold and was required to perform the project under certain constraints, namely being constrained to only 6,000 rows of data on which to build the model, but had complete discretion regarding the number of features in the model and the modeling technique applied.

The task is to predict if a person's income is in excess of $50,000 given certain profile information, and more specifically to generate predicted probabilities of income being **above** $50,000 for each row in the test set.

 Descriptions of the data can be found [here](https://archive.ics.uci.edu/ml/datasets/adult).

This project involved performing exploratory data analysis, identifying data cleaning steps. Because I was unconstrained by the number of features, I engineered my data using Polynomial Features to capture potential interaction terms.

We used pipelines and grid searches to select models and identify the best model parameters.

Classification models employed, included:
1. Logistic regression
2. Decision Trees
3. Bagging Classifier
4. Random Forest
5. AdaBoost Classifier
6. Support Vector Machines

The Bagging Classifier proved to be our best model and when predictions were applied to an unseen, holdout portion of the dataset, our model achieved an ROC AUC score of 96%.
