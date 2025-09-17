#Goal:

We want to build a simple linear regression model:

Co2 =α+β×(Feature)+ϵ

Understand the data
FuelConsumption.csv:
You will use a fuel consumption dataset, FuelConsumption.csv, which contains model-specific fuel consumption ratings and estimated carbon dioxide emissions for new light-duty vehicles for retail sale in Canada. Dataset source.

MODEL YEAR e.g. 2014
MAKE e.g. VOLVO
MODEL e.g. S60 AWD
VEHICLE CLASS e.g. COMPACT
ENGINE SIZE e.g. 3.0
CYLINDERS e.g 6
TRANSMISSION e.g. AS6
FUEL TYPE e.g. Z
FUEL CONSUMPTION in CITY(L/100 km) e.g. 13.2
FUEL CONSUMPTION in HWY (L/100 km) e.g. 9.5
FUEL CONSUMPTION COMBINED (L/100 km) e.g. 11.5
FUEL CONSUMPTION COMBINED MPG (MPG) e.g. 25
CO2 EMISSIONS (g/km) e.g. 182
Your task will be to create a simple linear regression model from one of these features to predict CO2 emissions of unobserved cars based on that feature.

#Features:

<img width="573" height="440" alt="Screenshot 2025-09-17 at 21 08 55" src="https://github.com/user-attachments/assets/fc3cf1ce-efe0-4158-ac84-5509e8fe49cd" />

<img width="581" height="438" alt="Screenshot 2025-09-17 at 21 09 33" src="https://github.com/user-attachments/assets/ab3be057-7c6f-44d4-83d5-762f64788558" />

Three car groups each have a strong linear relationship between their combined fuel consumption and their CO2 emissions. Their intercepts are similar, while they noticeably differ in their slopes.

# Regressionmodel

Model evaluation
You can compare the actual values and predicted values to calculate the accuracy of a regression model. Evaluation metrics play a key role in the development of a model, as they provide insight into areas that require improvement.

There are different model evaluation metrics, let's use MSE here to calculate the accuracy of our model based on the test set:

Mean Absolute Error: It is the mean of the absolute value of the errors. This is the easiest of the metrics to understand since it’s just an average error.

Mean Squared Error (MSE): MSE is the mean of the squared error. In fact, it's the metric used by the model to find the best fit line, and for that reason, it is also called the residual sum of squares.

Root Mean Squared Error (RMSE). RMSE simply transforms the MSE into the same units as the variables being compared, which can make it easier to interpret.

R-squared is not an error but rather a popular metric used to estimate the performance of your regression model. It represents how close the data points are to the fitted regression line. The higher the R-squared value, the better the model fits your data. The best possible score is 1.0 and it can be negative (because the model can be arbitrarily worse).

<img width="607" height="438" alt="Screenshot 2025-09-17 at 21 08 41" src="https://github.com/user-attachments/assets/80b035be-e9ca-46d6-8f6e-1dfbb1798ffa" />

#Regression model result over the test data instead of the training data

<img width="579" height="428" alt="Screenshot 2025-09-17 at 21 17 17" src="https://github.com/user-attachments/assets/6b0af0ed-be48-4b04-a030-68241e859b10" />

