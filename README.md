# LAB-TES ANSWERS

Question 2

2.1
A prediction value of -1 means the perceptron model classified the book `[3, 2]` as belonging to the negative class.
In binary terms, it didn’t meet the threshold for a positive label (`1`), indicating it does not share features with positive samples.

2.2
From the output, the total number of misclassifications observed across 10 epochs is the sum of`perceptron.errors_.
According to the code, the error count decreases to zero by epoch 7, meaning all samples are correctly classified after that point.

2.3
The error rate reaches zero by the seventh epoch because the perceptron successfully finds a linear boundary that separates the two classes.
Once it finds this separating hyperplane, no more updates to the weights are needed.

Question 3

3.1
The SVM classifier provided a clearer separation of the two classes because it maximizes the margin between data points and the decision boundary, making it more robust to overlapping features.
3.2
SVMs with kernel functions can transform non-linear data into higher-dimensional spaces where the classes become linearly separable.
Logistic Regression cannot do this without explicit feature transformations.

Question 4

4.1
Feature scaling ensures all features contribute equally to model training, especially for distance-based algorithms like SVMs or K-Means.
Without scaling, features with larger numeric ranges dominate the learning process.

4.2
If categorical variables remain unencoded, the model will treat them as numeric values or reject them, leading to misinterpretation of relationships and **incorrect learning patterns**.

Question 5

5.1
Typically, the first two principal components capture around 95–98% of the total variance (depending on dataset).
They retain most information while reducing the number of features.

5.2
PCA is effective for visualizing high-dimensional data because it compresses many correlated features into a few uncorrelated components, allowing patterns and clusters to be easily seen in 2D or 3D space.



Question 6

6.1
Cross-validation provides a more reliable performance estimate because it tests the model on multiple folds of data, reducing the bias of a single random train/test split.

6.2
Hyperparameter tuning finds the most generalizable configuration for a model, reducing overfitting by preventing the model from memorizing the training data.

Question 7

7.1
Ensemble models outperform individual models because they combine multiple learners, reducing variance and bias, and improving stability through methods like bagging or boosting.

7.2
Based on results, bagging (Random Forest) performed slightly better in accuracy and stability because it averages many trees, reducing variance.
Boosting (AdaBoost) can sometimes overfit, but it’s stronger when weak learners need to be corrected iteratively.

Question 8

8.1
The sentiment prediction for “The book was good” is positive (1), as seen in the model output using TF-IDF and Logistic Regression.
8.2
Text preprocessing (tokenization, stopword removal, lemmatization) removes noise and irrelevant words, helping the model focus on meaningful features that improve classification accuracy.

Question 9

9.1
The Random Forest model achieved a lower RMSE compared to Linear Regression because it captures non-linear relationships and interactions between variables.
9.2
Random Forests outperform Linear Regression when the dataset is non-linear or complex, since they build multiple trees that can model irregular patterns without requiring linear assumptions.

Question 10

10.1
The resulting clusters from K-Means roughly align with the true Iris species, but not perfectly.
This is because K-Means is unsupervised and relies on feature similarity, not actual class labels.

10.2
Clustering is an unsupervised learning method because it groups data based on internal structure without using predefined class labels it discovers patterns autonomously.


