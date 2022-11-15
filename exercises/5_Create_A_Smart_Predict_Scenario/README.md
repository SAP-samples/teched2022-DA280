# Exercise 5 - Create a Smart Predict Scenario 

In this exercise, you will create a Smart Predict scenario with the energy price as an influencer.

## Creating a Smart Predict Scenario

1. Click on the Predictive Scenario Icon on the left in the navigation panel.

![Screenshot1](https://github.com/SAP-samples/teched2022-DA280/blob/main/exercises/5_Create_A_Smart_Predict_Scenario/images/Screenshot1.PNG)

2. Create a new Time Series Forecast.

![Screenshot2](https://github.com/SAP-samples/teched2022-DA280/blob/main/exercises/5_Create_A_Smart_Predict_Scenario/images/Screenshot2.PNG)

3. Navigate into your My Files folder, choose a name for the predictive scenario e.g. Predictive Liquidity Planning and press "OK" to save it.

![Screenshot3](https://github.com/SAP-samples/teched2022-DA280/blob/main/exercises/5_Create_A_Smart_Predict_Scenario/images/Screenshot3.PNG)

4. Click on the marked icon to choose a data source model for the predictive scenario.

![Screenshot4](https://github.com/SAP-samples/teched2022-DA280/blob/main/exercises/5_Create_A_Smart_Predict_Scenario/images/Screenshot4.PNG)

5. Navigate to your My Files folder and choose your "COPY_SAP_FI_CLM_IM_LIQUIDITY_PLANNING" model by clicking on it.

![Screenshot5](https://github.com/SAP-samples/teched2022-DA280/blob/main/exercises/5_Create_A_Smart_Predict_Scenario/images/Screenshot5.PNG)

6. In the settings panel on the right, choose "Amount" as a measure, "Energy Expenses" as an account, "Time" as a date, "12" for the number of periods and "Company Code" & "Transaction Currency" for the Entity.

![Screenshot6](https://github.com/SAP-samples/teched2022-DA280/blob/main/exercises/5_Create_A_Smart_Predict_Scenario/images/Screenshot6.PNG)

7. Turn on the toggle to convert negative forecast values to zero and choose "Amount" and "Energy Price / GWh" in the dropdowns "Include As Influencer" and click on the confimation Icon.

8. Afterwards click on "Train & Forecast.

![Screenshot7](https://github.com/SAP-samples/teched2022-DA280/blob/main/exercises/5_Create_A_Smart_Predict_Scenario/images/Screenshot7.PNG)

8. Click on the "Save" icon to save your Smart Predict Scenario

![Screenshot18](https://github.com/SAP-samples/teched2022-DA280/blob/main/exercises/5_Create_A_Smart_Predict_Scenario/images/Screenshot18.PNG)

Your Smart Predict Scenario is created! Now you can review the results.






## Summary

Now that you have created a smart predict scenario you can continue to - [Exercise 6 - Create a Multi Action](../6_Create_A_Multi_Action/README.md)
