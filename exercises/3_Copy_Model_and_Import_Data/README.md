# Exercise 3 - Copy the planning model and load the data
In this exercise, we will copy the planning model from the sample content into our own folder and import the actual data and influencers from SAP Data Warehouse Cloud (DWC). For this, we will use an existing connection to DWC and create an data import job in the planning model.

## Exercise 3.1 Copy the planning model

1. First, we open the Files folder by clicking on "Files" on the left navigation panel.

![screenshot01](https://user-images.githubusercontent.com/112691476/196177480-bf012fcc-6033-414d-a58b-ad321af88a2e.png)

2. Next, we navigate to the public folder, where we can find the TechEd sample content.
This folder contains the story and data model which we will use as the basis for the next exercises.

![](/exercises/3_Copy_Model_and_Import_Data/images/screenshot02.png)


3. Therefore we copy the TechEd sample content by selecting the folder and clicking on the "Copy To" Icon on the top right.

![](/exercises/3_Copy_Model_and_Import_Data/images/screenshot03.png)
 
4. In the pop-up box we change the file name to TechEd2022_DA280_[yourlastname] and save the copy to My Files

![](/exercises/3_Copy_Model_and_Import_Data/images/screenshot04.png)

## Exercise 3.2 Import data

1. Now let's load the data from SAP Data Warehouse Cloud into our SAP Analytics Cloud (SAC) model and build a table on top of it. We navigate into our copied sample content folder and open the model.

2. We switch to the Data Management View of the model where we can create the Import Job.

![](/exercises/3_Copy_Model_and_Import_Data/images/screenshot06.png)

3. By clicking on "import data" we can choose whether to import data from a flat file, e.g. a csv or choose an existing connection to a data source to import data from. In our case, we already have a connection to DWC so we select "Data source".

![](/exercises/3_Copy_Model_and_Import_Data/images/screenshot07.png)


4. In the pop-up window we choose OData Services.

![](/exercises/3_Copy_Model_and_Import_Data/images/screenshot08.png)

5. Next, we are prompted to select a connection from the dropdown list. We choose "DWC_TechEd_DA280_Union" as shown in the screenshot and click on "Next".

![](/exercises/3_Copy_Model_and_Import_Data/images/screenshot09.png)

6. Now we create a new query for the OData Service and set the name to "V_Union_Actuals_and_Influencer" and select the corresponding table. Proceed with "Next".

![](/exercises/3_Copy_Model_and_Import_Data/images/screenshot10.png)


7. In this view we can see the dimensions and measures the table consists of. We could select individual dimensions and measures in the query however in this case, we want to include the whole table. Using drag and drop we can simply drag the table to the "Selected Data" area and drop it there. Now all 10 dimensions and measures are included in the result set. To confirm we press "Create". The system now sets up the import job in the background and lets us know as soon as it is created.

![](/exercises/3_Copy_Model_and_Import_Data/images/screenshot11.png)


8. Once the import job is created we can set up the import.


![](/exercises/3_Copy_Model_and_Import_Data/images/screenshot12.png)

9. The first view which is shown is the data preparation step. Here we could resolve data quality issues before the mapping step, but also wrangle data and make edits such as renaming columns, create transformations, etc. In our case, we can skip this step and proceed with the mapping.

![](/exercises/3_Copy_Model_and_Import_Data/images/screenshot13.png)

10. In the next step, the mapping between source and target columns is defined. The system already did most of the mapping for us, so we only have to map the "TIMEMONTH" column to the "Time" column. This can be done by dragging the TIMEMONTH column onto the blank source space of the Time column. Once this is done, we click on "Next".

![](/exercises/3_Copy_Model_and_Import_Data/images/screenshot14.png)

11. In this view, we can add descriptions by mapping the description members of our source column to respective target column. The mapping is shown in the screenshot below. Once this is done, we click on Next. The system now validates the mappings and if no errors are found we can proceed to run the import.

![](/exercises/3_Copy_Model_and_Import_Data/images/screenshot15.png)

12. We click on "Run Import" and choose "Finish". 

![](/exercises/3_Copy_Model_and_Import_Data/images/screenshot16.png)

13. The data is now being imported into SAC. Once the process is finished, the status bar on the right shows information about the date and duration time of the import process and number of rows which have been imported. 

![](/exercises/3_Copy_Model_and_Import_Data/images/screenshot17.png)

Thereby, you successfully imported data from DWC to SAC, congratulations!


## Summary

Now let's have a look how we can build a table on top of that to carry out our Liqudity Planning.
Continue to - [Exercise 4 - Story_Building](../4_Story_Building/Readme.md)

