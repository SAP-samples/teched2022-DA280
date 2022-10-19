# Exercise 1 - Acquiring Data from SAP Data Warehouse Cloud

In this exercise, we first look for external data on energy prices in the Data Marketplace of SAP Data Warehouse Cloud. We will then combine this data with our internal cash flow statement actuals and create a consumable view. Finally, we create a connection from SAP Analytics Cloud to SAP Data Warehouse Cloud that will allow us to easily transfer the data into a planning model. 

## Exercise 1.1 Adding External Data via Data Marketplace

After completing these steps you will have created an Analytical Dataset in SAP Data Warehouse Cloud, which combines external data from Data Marketplace with internal actuals. 

1. 
<br>![](/exercises/ex1/images/01_01_0010.png)

2.	Insert this line of code.
```abap
response->set_text( |Hello World! | ). 
```



## Exercise 1.2 Connect SAC to DWC

After completing these steps you will have...

1.	Enter this code.
```abap
DATA(lt_params) = request->get_form_fields(  ).
READ TABLE lt_params REFERENCE INTO DATA(lr_params) WITH KEY name = 'cmd'.
  IF sy-subrc <> 0.
    response->set_status( i_code = 400
                     i_reason = 'Bad request').
    RETURN.
  ENDIF.

```

2.	Click here.
<br>![](/exercises/ex1/images/01_02_0010.png)


## Summary

You've now ...

Continue to - [Exercise 2 - Exercise 2 Description](../ex2/README.md)

