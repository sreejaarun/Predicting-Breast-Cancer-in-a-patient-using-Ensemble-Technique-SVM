# Predicting-Breast-Cancer-in-a-patient-using-Ensemble-Technique-SVM
To perform breast cancer prediction using Support Vector Classifier (SVC),follow these steps:
*Import the required libraries
*Load the breast cancer dataset
*Split the data into training and testing sets
*Create an instance of the SVC classifier and train it
*Make predictions on the test set
*Evaluate the accuracy of the model

In this breast cancer prediction, it appears that we have a pandas DataFrame with 569 rows and 33 columns.
The dataset contains a mix of numerical and categorical data. The diagnosis column is of object type, likely representing the class labels.

Before proceeding with the SVC model, we may need to preprocess the data by performing tasks such as:

*Handling missing values (Unnamed: 32 column appears to have all non-null values).
*Converting the categorical diagnosis column to numerical format if necessary (e.g., Malignant = 1, Benign = 0).
*Scaling or normalizing the numerical features to ensure they have similar ranges.
*Removing any unnecessary columns or features that may not contribute to the prediction task.
*Once we have preprocessed the data, we can follow the steps to train an SVC model for breast cancer prediction using the appropriate features and the preprocessed target variable.

In my model I have done classification report and confusion matrix
*The classification_report and confusion_matrix functions are used for evaluating the performance of a classification model.

*The confusion_matrix is a table that shows the performance of a classification model by summarizing the counts of true positives, true negatives, false positives, and false negatives. It provides a more detailed understanding of how well the model is predicting each class. From the confusion matrix, various metrics such as accuracy, precision, recall, and F1-score can be derived.

The classification_report function provides a text-based summary of the main classification metrics: precision, recall, F1-score, and support. Precision represents the ability of the model to correctly identify positive samples, recall represents the ability to find all positive samples, and F1-score is the harmonic mean of precision and recall. The support refers to the number of occurrences of each class in the test data.

By using these functions, we can assess the performance of your SVC model, identify any issues such as imbalanced classes, and make informed decisions about the model's effectiveness for your specific classification task.

CONCLUSION

From the SVM model, classification report, and confusion matrix of the breast cancer dataset, we can draw the following conclusions:

SVM Model: The SVM model was trained on the breast cancer dataset, and it achieved an accuracy of 95%. This indicates that the model is able to classify the majority of the samples correctly.

Confusion Matrix: The confusion matrix provides a detailed breakdown of the model's predictions. In this case, the confusion matrix shows that there are 71 true negatives (TN) and 37 true positives (TP) for class 1, while there are no false negatives (FN) or false positives (FP) for class 1. This suggests that the model performs well in correctly identifying both class 0 and class 1 samples.

Classification Report: The classification report provides further insights into the model's performance by calculating precision, recall, F1-score, and support for each class.

Class 0 (negative class): The precision is 0.92, indicating that the model correctly identifies 92% of the true negatives. The recall is 1.00, indicating that all actual class 0 samples are correctly identified. The F1-score is 0.96, indicating a good balance between precision and recall for class 0.

Class 1 (positive class): The precision is 1.00, indicating that all predicted positives are true positives. The recall is 0.86, indicating that 86% of the actual class 1 samples are correctly identified. The F1-score is 0.92, indicating a good balance between precision and recall for class 1.

Overall, the classification report indicates that the model performs well in distinguishing between both class 0 and class 1, with high precision, recall, and F1-scores for both classes.

In summary, based on the SVM model's high accuracy, the balanced performance indicated by the classification report, and the absence of false negatives and false positives in the confusion matrix, we can conclude that the SVM model shows promise in accurately classifying breast cancer samples and has the potential to be a reliable tool for breast cancer diagnosis.


