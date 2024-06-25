# Consumption_Model
Predicting the Material consumption using linear regression 
**Stepwise flow of the model **

Step 1: Loading Required Libraries
We begin by loading the necessary Python libraries such as pandas and numpy for data manipulation, and sklearn for machine learning tasks.

Step 2: Loading Data
We load the historical data from a CSV file into a DataFrame. This DataFrame contains information on variables such as temperature, slag analysis, melted steel weight, desired grade, presence of other alloys like Ti, Si, Ca, and the amount of aluminum added.

Step 3: Simulating Aluminum Loss
We compute the simulated loss of aluminum in the slag based on the historical data. The historical data might not contain this information explicitly, so we simulate it assuming a 15-25% loss.

Step 4: Computing Aluminum Yield
We calculate the actual aluminum yield by subtracting the simulated aluminum loss from the amount of aluminum added.

Step 5: Training a Linear Regression Model
We train a linear regression model using LinearRegression to predict the aluminum yield based on the given variables (temperature, slag analysis, melted steel weight, desired grade, presence of Ti, Si, Ca).

Step 6: Predicting Aluminum Yield
We use the trained model to predict the aluminum yield for the historical data.

Step 7: Model Evaluation
We evaluate the performance of the model by calculating the root mean squared error (RMSE) between the predicted aluminum yield and the actual aluminum yield from the historical data.
