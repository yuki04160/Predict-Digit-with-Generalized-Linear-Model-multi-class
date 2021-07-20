# Predicting ![Handwritten Digit](https://user-images.githubusercontent.com/74026413/126390004-dce88dd4-b731-47ba-9364-c9448a8c9a4c.png)
To predict handwritten digit (0~9), I built a Multiclass Logistic Regression in R using Kaggle dataset [mnist_test](https://www.kaggle.com/oddrationale/mnist-in-csv), which is an image pixel dataset.
## Inrtroduction
Generalized Linear Model (GLM) is a flexible generalization of ordinary linear regression. To be more specific, GLM allows for response variables that have error distribution models other than a normal distribution. In this project, I applied one type of GLM, Logistic Regression Model, to predict handwritten digits. Since it is a multiclass classification problem, I utilized Multiclass Logistic Regression, which is also called Multinomial Logistic Regression or Softmax Regression.
## Exploratory Data Analysis
   - Plot images
   - Plot digit labels distribution
## Data Preprocessing
   - Examine missing value
   - Split into training (0.8) and test (0.2)
## Data Modeling
Multiclass logistic regression
   - I built 10 logistic regression models, one per digit.
   - I used the Softmax function to transform unrelated probabilities into a probability distribution over 10 digits.
## Multiclass Classification Model Evaluation
   - Overall accuracy
   - True Positive Rate (sensitivity/ recall) of each digit
## Conclusion
To sum up, I trained 10 models, one per digit, and used the Softmax function to turn unrelated probabilities into related probabilities. Finally, with predicted results, I built a confusion matrix and calculated the overall accuracy. From the model results, I found that digit 1 has the highest TPR, above 90%, and digits 0 and 7 also have high TPR, above 80%. However, digits 5 and 8 have lower TPR, only around 65%. That is to say, the model can highly correctly recognize handwritten digits of 1, 0, and 7, but can not recognize handwritten digits of 5 and 8 very well.
