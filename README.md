# Predicting Handwritten Digit with Multi-class Logistic Regression
To predict handwritten digits (0~9), I built a Multi-class Logistic Regression in R using Kaggle dataset [mnist_test](https://www.kaggle.com/oddrationale/mnist-in-csv), which is an image pixel dataset.
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
2. Create Softmax Function (the function can turn a vector of K real values into a vector of K real values that sum to 1)
## Multiclass Classification Model Evaluation
   - Accuracy
   - True Positive Rate (Sensitivity/ Recall) of each class/ digit
## Conclusion
To sum up, I trained 10 models, one per digit, and used the Softmax function to turn unrelated probabilities into related probabilities. Finally, with predicted results, I built a confusion matrix and calculated the overall accuracy. From the model results, I found that digit 1 has the highest TPR, above 90%, and digits 0 and 7 also have high TPR, above 80%. However, digits 5 and 8 have lower TPR, only around 65%. THat is to say, the model can highly correctly recognize handwritten digits of 1, 0, and 7, but can not recognize handwritten digits of 5 and 8 very well.
