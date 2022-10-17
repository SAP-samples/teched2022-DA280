# Exercise 1 - Exercise 1 Description

In this exercise, we will create...

## Exercise 1.1 Sub Exercise 1 Description

After completing these steps you will have created...

1. First, we open the Files folder by clicking on "Files" on the left navigation panel.

![screenshot01](https://user-images.githubusercontent.com/112691476/196177480-bf012fcc-6033-414d-a58b-ad321af88a2e.png)

2. Next, we navigate to the public folder, where we can find the TechEd sample content.
This folder contains the Story and data model which we will use as the basis for the next excercises.

![](/exercises/4_Story_Building/images/screenshot02.png)


3. Therefore we copy the TechEd sample content by selecting the folder and clicking on the "Copy To" Icon on the top right.

![](/exercises/4_Story_Building/images/screenshot03.png)
 
4. In the pop-up box we change the file name to TechEd2022_DA280_[yourlastname] and save the copy to My Files / Public

![](/exercises/4_Story_Building/images/screenshot04.png)

5. Now let's load the data from Data Warehouse Cloud into our SAP Analytics Cloud Model and build a table on top of it. We nagivate into our copied sample content folder and open the Model.


6. We switch to the Data Management View of the model where we can create the Import Job.

![](/exercises/4_Story_Building/images/screenshot06.png)




## Exercise 1.2 Sub Exercise 2 Description

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

