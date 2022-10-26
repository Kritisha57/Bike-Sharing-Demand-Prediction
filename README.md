# Bike Sharing Demand Prediction-Capstone Project
Currently Rental bikes are introduced in many urban cities for the enhancement of mobility comfort. It is important to make the rental bike available and accessible to the public at the right time as it lessens the waiting time. Eventually, providing the city with a stable supply of rental bikes becomes a major concern. The crucial part is the prediction of bike count required at each hour for the stable supply of rental bikes. The goal is to design different Machine Learning models and come up with the model which gives the best prediction of rented bike count required to be supplied at each hour. Before designing any ML model, we require to clean the data and draw significant insights from the data. To begin with we view the dataset including its description, various columns, number of null values, different categorical variables, unique value count, shape of the dataset and different statistical parameters. We begin by removing the null values if any. Then we plot the distributions of each variable to see how the data is distributed. We get an idea about the skewness of the data. Ideally, we want our data to have a normal distribution. If there is skewness in the data we go for feature transformation. Visualizing different kinds of transformation on the skewed variables helps you to determine the best transformation for your features. We can check the numerical value of skewness of the variables using the .skew() method. We also plot box plot of the features to check the outliers in the data. Outliers play a significant role in data analysis as they effect the statistical parameters. Then we plot the correlation heatmap to check for collinear features. Since collinearity is not desired in the data, we linearly combine the collinear features or drop them. Variance Inflation Factor (VIF) is used to detect the presence of multicollinearity. Variance inflation factors (VIF) measure how much the variance of the estimated regression coefficients are inflated as compared to when the predictor variables are not linearly related. In our project, Year and Dew point temperature have t he highest VIFs hence they’re dropped. Moving ahead, we analyze the categorical variables and perform one hot encoding for conversion. The original categorical columns are dropped and we get our final clean dataset. A feature importance graph is plotted to show which features contribute the most to our model. Then we perform the splitting of the data into train-test sets and perform feature scaling. Then we apply LR, Decision Tree, Random forest regression, XG Boost regression, Bagging and Stacking models to get the best model for our business problem. We calculate the evaluation metrics R2 score, MSE, RMSE and Cross validation accuracy for each model. Then a model comparison chart is plotted to compare the metrics. Stacking Regressor gives the best results of all the models for the given business problem.
