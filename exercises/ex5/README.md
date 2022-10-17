
# Level 1 Heading

In this exercise, you will...

## Level 2 Heading

1. Click on the Predictive Scenario Icon on the left in the navigation panel.

![Screenshot1](https://github.com/SAP-samples/teched2022-DA280/blob/main/exercises/ex5/images/Screenshot1.PNG)

2. Create a new Time Series Forecast

![Screenshot2](https://github.com/SAP-samples/teched2022-DA280/blob/main/exercises/ex5/images/Screenshot2.PNG)

3. Navigate into your folder, choose a name for the predictive scenario and press "OK" to save it.

![Screenshot3](https://github.com/SAP-samples/teched2022-DA280/blob/main/exercises/ex5/images/Screenshot3.PNG)

4. Click on the marked icon to choose a data source model for the predicitve scenario.

![Screenshot4](https://github.com/SAP-samples/teched2022-DA280/blob/main/exercises/ex5/images/Screenshot4.PNG)

5. Navigate to your folder and choose the "COPY_SAP_FI_CLM_IM_LIQUIDITY_PLANNING" model by clicking on it.

![Screenshot5](https://github.com/SAP-samples/teched2022-DA280/blob/main/exercises/ex5/images/Screenshot5.PNG)

6. In the settings panel on the right, choose "Amount" as a measure, "Energy Expenses" as an account, "Time" as a date, "12" for the number of periods and "Company Code" & "Transaction Currency" for the Entity.

![Screenshot6](https://github.com/SAP-samples/teched2022-DA280/blob/main/exercises/ex5/images/Screenshot6.PNG)

7. Turn on the toggle to convert negative forecast values to zero and choose "Amount" and "Energy Price / GWh" in the dropdowns "Include As Influencer" and click on the confimation Icon.

8. Afterwards click on "Train & Forecast.

![Screenshot7](https://github.com/SAP-samples/teched2022-DA280/blob/main/exercises/ex5/images/Screenshot7.PNG)

Your Smart Predict Scenario is created! Now you can review the results.




2.	Insert this code.
``` abap
 DATA(params) = request->get_form_fields(  ).
 READ TABLE params REFERENCE INTO DATA(param) WITH KEY name = 'cmd'.
  IF sy-subrc <> 0.
    response->set_status( i_code = 400
                     i_reason = 'Bad request').
    RETURN.
  ENDIF.
```

## Summary

Now that you have ... 
Continue to - [Exercise 1 - Exercise 1 Description](../ex1/README.md)
