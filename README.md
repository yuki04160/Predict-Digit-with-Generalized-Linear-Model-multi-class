# Predicting Handwritten Digit with Multi-class Logistic Regression
To predict handwritten digits, I built a Multi-class Logistic Regression in R using Kaggle dataset [mnist_test](https://www.kaggle.com/oddrationale/mnist-in-csv).
## Inrtroduction
Generalized Linear Model (GLM) is a flexible generalization of ordinary linear regression. To be more specific, GLM allows for response variables that have error distribution models other than a normal distribution. In this project, I applied one type of GLM, Logistic Regression Model, to predict handwritten digits. Since it is a multiclass classification problem, I utilized Multi-class Logistic Regression, which is also called Multinomial Logistic Regression or Softmax Regression.
## Exploratory Data Analysis
1. Plot Images
2. Plot Digit Labels Distribution
## Data Preprocessing
1. Examine Missing Value
2. Split into Training (0.8) and Test (0.2)
## Data Modeling
1. Build 10 Logistic Regression Models (one per digit)
2. Create Softmax Function
   - THe function turns a vector of K real values into a vector of K real values that sum to 1.
## Multiclass Classification Model Evaluation
   - Accuracy
   - True Positive Rate (Sensitivity/ Recall) of each digit
## Conclusion
To sum up, I trained 10 models, one per digit. Then, I used each model to predict on the test dataset, which contains 3000 images, so I got a total of 10x3000=30000 probabilities (10 probabilities per image). For each image, I used the Softmax function to turn those 10 unrelated probabilities into 10 related probabilities. Based on the 10 related probabilities, the predicted digit for each image is the one associated with the maximum probability. Finally, with predicted results, I built a confusion matrix and calculated the overall accuracy.
