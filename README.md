# Predicting Handwritten Digit with Multi-class Logistic Regression
To predict handwritten digits, I built a Multi-class Logistic Regression in R using Kaggle dataset [mnist_test](https://www.kaggle.com/oddrationale/mnist-in-csv).
## Inrtroduction
Generalized Linear Model (GLM) is a flexible generalization of ordinary linear regression. To be more specific, GLM allows for response variables that have error distribution models other than a normal distribution. In this project, I applied one type of GLM, Logistic Regression Model, to predict handwritten digits. Since it is a multiclass classification problem, I utilized Multi-class Logistic Regression, which is also called Multinomial Logistic Regression or Softmax Regression.
## EDA
1. Plot Images
2. Examine Missing Value
3. Split into Training (0.8) and Test (0.2) datasets
## Data Modeling
1.
2.
3.


The "mnist_test" is a dataset containing 10,000 of 28x28 grayscale images. Each image is encoded as a row of 784 (28x28) integer values between 0 and 255 indicating the brightness of each pixel. The label associated with each image is encoded as an integer value between 0 and 9. Overall, there are 785 columns in the dataset, where the first column corresponds to the digit labels (0-9), and the remaining 784 columns correspond to the pixel-values of the associated image. To predict a digit, the first column is used as the target variable.
