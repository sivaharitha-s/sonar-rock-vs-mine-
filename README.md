Sonar Data Classification

This project implements multiple machine learning models to classify sonar data. The dataset contains numerical values representing sonar signals, with labels indicating whether the object is a rock (0) or a mine (1).

Models Used

K-Nearest Neighbors (KNN)

Random Forest Classifier

Decision Tree Classifier

Support Vector Machine (SVM)

Logistic Regression

Dataset

The dataset used is Copy of sonar data.csv, where the target variable is in the last column (column index 60). The labels are converted from 'R' (Rock) and 'M' (Mine) to binary values (0 and 1, respectively).

Data Preprocessing

Load the dataset using Pandas.

Convert categorical labels into numerical values.

Split the dataset into training and testing sets (80% train, 20% test).

Perform data visualization using Seaborn pair plots to analyze class separation.

Model Training and Evaluation

Train the models on the training dataset.

Make predictions on the test dataset.

Compare the accuracy scores of different models.

Accuracy Scores

The following accuracy scores are obtained on the test dataset:

print("Logistic Regression:", reg.score(test_x, test_y))
print("KNN:", knn.score(test_x, test_y))
print("Random Forest:", random.score(test_x, test_y))
print("Decision Tree:", decision.score(test_x, test_y))
print("SVM:", svmm.score(test_x, test_y))

Results:
logistic 0.7857142857142857
knn 0.8571428571428571
random 0.8333333333333334
decision 0.7142857142857143
svm 0.7857142857142857

The pair plot visualization suggests overlapping data points, making KNN a suitable model. The classification accuracy of each model helps in determining the best-performing one.
