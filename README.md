# Inventory Depletion Prediction and Alert System using Exponential Weighted Moving Average (EWMA)
The provided code is for simulating inventory management using Exponential Weighted Moving Average (EWMA). Initially, it creates a mock inventory dataset for security reasons.

Setup dates: The code sets the dates from '2024-01-01' to '2024-01-31'.
Generate product list: It generates a list of 50 products named 'product_1' to 'product_50'.
Generate inventory data: For each product, it creates a randomized inventory data. The starting inventory is a random number between 100 and 300. The daily depletion is also randomized based on the inventory.

After creating the mock data, the code applies the EWMA model to predict inventory depletion:

Apply EWMA: It applies the EWMA model on the daily usage data of each product. The EWMA gives more weight to the recent data, hence, it is a good model for predicting inventory depletion.
Predict depletion: For each product, it calculates the expected days until the inventory runs out based on the last inventory and the last EWMA value.
Alert: If the expected depletion time is less than or equal to 3 days, it prints an alert message.
