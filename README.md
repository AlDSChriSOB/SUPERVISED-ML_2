# SUPERVISED-ML_2
This script investigates Naive Bayes for classification tasks, using the classic "Golf" dataset to predict whether or not someone will play tennis based on weather conditions.

Data Analysis and Visualization

The code defines sample weather data (outlook, temperature, humidity, wind) and corresponding labels (play tennis or not) for 14 instances.

Data Preprocessing

Label encoding is applied to convert categorical features (outlook, temperature, humidity, wind, play) into numerical representations suitable for the Naive Bayes model.
Naive Bayes Model

Model Definition and Training:

A Gaussian Naive Bayes classifier is created using sklearn.naive_bayes.GaussianNB. This assumes a Gaussian (normal) distribution for continuous features.
The model is trained on the encoded features and labels.
Prediction:

The code demonstrates how to make a prediction for a new data point (Overcast, Mild, Normal, Strong) using classifier.predict.
Evaluation:

Test Set Evaluation:

The data is split into training (70%) and testing (30%) sets using sklearn.model_selection.train_test_split.
The model is retrained on the training set.
Predictions are made on the test set, and accuracy is calculated using sklearn.metrics.accuracy_score.
Cross-Validation:

sklearn.model_selection.cross_val_score is used for 5-fold cross-validation to assess model generalizability. Average accuracy across folds is reported.
Conclusion

This script explores how Naive Bayes can be used for classification. It demonstrates data encoding, prediction, and evaluation using both a test set and cross-validation. By analyzing the results, you can gain insights into the model's performance on unseen data.
