# Linear-Regression---GPA-Predictor
A linear regression model for predicting GPA from scores. It is an implementation of the linear regression formula involving the manipulation of matrices.

**gpa_generator** generates a uniform random distribution scores alongside their corresponding GPAs. It is used to generate **gpa_train_x_scores** where 'x' represents the dataset length. Also a test dataset, **gpa_test_score** is used to compare the accuracy of various datasets.

In **gpa_linear_regression**, the dataset is first split into two, training(X) and target(y). Using the formula above the weights(theta) are initialised to zero and a bias values (ones) is appended into the training dataset to get the form of mx + c, where m are the weights, x is the training dataset, and c is the bias values.

[Gradient descent](https://towardsdatascience.com/linear-regression-using-gradient-descent-97a6c8700931) is then calculated. Learning rate is varied while keeping the number of iterations constant. An ideal learning rate is found to be 0.5. Iterations are then varied while learning rate is kept constant. All results are shown using graphs.

The above steps are carried out for the different dataset sizes and upon inspection (i.e using plots and using mean squared error as the measure of accuracy. Datasets of 2000, 5000 gave the best accuracy(the smaller the MSE, the better the accuracy).

fastai library is then used to implement the GPA Predictor in **gpa_predictor - fast_ai**.

***Results***
T**gpa_linear_regression** normalised by the scaling 
