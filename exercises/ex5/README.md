
# Level 1 Heading

In this exercise, you will...

## Level 2 Heading

1. Click on the Predictive Scenario Icon on the left in the navigation panel.

![Screenshot1](https://github.com/SAP-samples/teched2022-DA280/blob/main/exercises/ex5/images/Screenshot1.PNG)

2. Create a new Time Series Forecast

![Screenshot2](https://github.com/SAP-samples/teched2022-DA280/blob/main/exercises/ex5/images/Screenshot2.PNG)

1.	Click here.
<br>![](/exercises/ex0/images/00_00_0010.png)


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
