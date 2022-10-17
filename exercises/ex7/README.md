# Level 1 Heading

In this exercise, you will create a Data Action to clean up the version data before running the prediction.

## Level 2 Heading

After completing these steps you will have created a Data Action with an advanced formular step to clean up the version data. After that, you can run the predictive scenario for the energy costs.

1.	Click here.
![Deletion_2_new](https://user-images.githubusercontent.com/112930664/196192889-0e7c121b-afda-4c21-a38d-649df4a198b0.png)

![Deletion_4](https://user-images.githubusercontent.com/112930664/196191988-949a31e3-69e7-4948-bc25-62ba93ebff2f.png)

![Deletion_7](https://user-images.githubusercontent.com/112930664/196192069-a5cefd6a-a75d-46d7-9c14-249debc4794c.png)

![Deletion_8](https://user-images.githubusercontent.com/112930664/196192146-b79fbb57-b805-43ea-ae48-9b92275f96ed.png)

![Deletion_9](https://user-images.githubusercontent.com/112930664/196192166-8a677bec-12be-4230-a513-295290e3a6ca.png)

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
