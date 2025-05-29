🎯 Objective
To implement and understand simple and multiple linear regression using Scikit-learn with a real-world dataset, and evaluate model performance.

🛠️ Tools Used
Pandas: For handling and manipulating the dataset.
Scikit-learn (sklearn): For implementing the regression model and evaluation metrics.
Matplotlib: For visualizing the regression results.

🔢 Dataset
The California Housing dataset is used.
It contains various features like median income, house age, population, etc., to predict the median house value.

📌 Step-by-Step Process
Step 1: Import and Load the Dataset
  ->Use fetch_california_housing from sklearn.datasets to load the housing data as a Pandas DataFrame.
  ->Explore the dataset to understand its structure and identify relevant features and target variable.

Step 2: Select Features and Target
  ->Choose meaningful input variables (e.g., MedInc, HouseAge, Population) as features.
  ->Use MedHouseVal (median house value) as the target variable to be predicted.

Step 3: Split Data into Training and Testing Sets
  ->Use train_test_split from sklearn.model_selection to divide the data.
  ->Typically, 80% is used for training and 20% for testing to evaluate how the model generalizes.

Step 4: Train the Linear Regression Model
  ->Create a LinearRegression object and fit it to the training data.
  ->This step estimates the intercept and coefficients (slopes) for the linear relationship.

Step 5: Evaluate the Model
  ->Use the model to predict values on the test set.
  ->Calculate evaluation metrics:
        *MAE (Mean Absolute Error): Average of absolute prediction errors.
        *MSE (Mean Squared Error): Average of squared prediction errors.
        *R² Score (Coefficient of Determination): Measures how well the model explains variance in the target.

Step 6: Interpret Model Coefficients
  ->Examine the intercept: baseline predicted value when all features are 0.
  ->Examine the coefficients: how each feature affects the predicted target.
  ->Positive coefficients increase the prediction; negative ones decrease it.

Step 7: Visualize the Results
  ->Use scatter plots to visualize actual vs. predicted values.
  ->For simple regression (one feature), plot the regression line over data points to see the fit.
  ->For multiple regression, plot predicted vs. actual values to assess model accuracy.

✅ Summary
This project demonstrates how to:
   ->Build a regression model using Scikit-learn
   ->Evaluate model performance with standard metrics
   ->Interpret and visualize results to understand relationships in the data
