

# Level 1 Heading

In this exercise, you will...

## Level 2 Heading

1. Click on the Multi Actions icon on the left in the navigation panel.

![Screenshot8](https://github.com/SAP-samples/teched2022-DA280/blob/main/exercises/ex6/images/Screenshot8.PNG)

2. Create a new Multi Action:

![Screenshot9](https://github.com/SAP-samples/teched2022-DA280/blob/main/exercises/ex6/images/Screenshot9.PNG)

3. Give your new Multi Action a name like shown in the Screenshot below.

![Screenshot10](https://github.com/SAP-samples/teched2022-DA280/blob/main/exercises/ex6/images/Screenshot10.PNG)

4. Now Click on the marked "+" icon to add a new step to your Multi Action. Choose the "Predictive Scenario" step.

![Screenshot11](https://github.com/SAP-samples/teched2022-DA280/blob/main/exercises/ex6/images/Screenshot11.PNG)

5. Give the new step a name. Afterwards choose the Predicitve Scenario which you have created in the step before.

![Screenshot12](https://github.com/SAP-samples/teched2022-DA280/blob/main/exercises/ex6/images/Screenshot12.PNG)

![Screenshot13](https://github.com/SAP-samples/teched2022-DA280/blob/main/exercises/ex6/images/Screenshot13.PNG)

6. For the Model choose "Model 1" and "Predictive Forecast as a version.

![Screenshot14](https://github.com/SAP-samples/teched2022-DA280/blob/main/exercises/ex6/images/Screenshot14.PNG)

7. Click on the "Add version Management Step" - icon in the toolbar to add an other step.

![Screenshot15](https://github.com/SAP-samples/teched2022-DA280/blob/main/exercises/ex6/images/Screenshot15.PNG)

8. Select a Model in the Panel on the right. Navigate to your folder and select the "COPY_SAP_FI_CLM_IM_LIQUIDITY_PLANNING" model by clicking on it.

![Screenshot16](https://github.com/SAP-samples/teched2022-DA280/blob/main/exercises/ex6/images/Screenshot16.PNG)

9. Choose Predictive Forecast as a Version and give this step a name like shown in the Screenshot:

![Screenshot17](https://github.com/SAP-samples/teched2022-DA280/blob/main/exercises/ex6/images/Screenshot17.PNG)

10. Click on the "Save" icon to save your Multi Action

![Screenshot18](https://github.com/SAP-samples/teched2022-DA280/blob/main/exercises/ex6/images/Screenshot18.PNG)


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
