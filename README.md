# Car-Price-Prediction
 Playing with regression models using a car data set from Kaggle.

My plan was to train a multiple linear regression model using a Car Prediction data set.

I followed the known steps of preprocessing such s removing variables that are not useful for prediction, one-hot-encoding categorical variables, and standardization of the numerical variables after the train-test split. To make these steps easier, I split the data into numerical and categorical data sets. After performing all the preprocessing steps (such as OHE and correlations), they were merged together into a single data set to be later split into training and testing sets. 

Because multiple linear regression was not performing well, I went for three other algorithms (SVR, decision tree, and random forest). I created a grid of hyperparameters that would be tested. The best model was chosen based on the R-squared score. **Random Forest** turned out to be the best one.

Food for thought and future improvements:
- I did not check for the usefulness of the categorical variables, only the numerical ones
- Maybe instrad of OHE, I should have used labeling (although that is not an ordinal data)
- OHE created many columns full of zeros, which could cause curse of dimensionality 
