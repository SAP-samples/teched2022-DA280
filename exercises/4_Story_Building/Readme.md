

# Exercise 4 - Story Building
Now that we have imported the data from SAP Datawarehouse Cloud (DWC) to our SAP Analytics Cloud (SAC) planning model, we can start building a table on top of the imported data. For that, we go to Files, navigate to our TechEd folder under My Files and open the story SAP__FI_CLM_LIQUIDITY_PLANNING. 

On the first page (Liquidity Overview), we can see the financial data visualized with different charts and key figures.
The second page (Liquidity Planning) is empty and we will now fill it. 

## Exercise 4.1 Create the first table


1. To add a table to the story, switch the story from View mode to Edit mode, select the tab Liquidity Planning and click on "Table" in the "Insert" toolbar.

![](/exercises/4_Story_Building/images/screenshot01.jpg)

2. We move the table to the left side of the story and resize its size as shown in the screenshot.

![](/exercises/4_Story_Building/images/screenshot02.jpg)

3. Let's also change the underlying data model of the table from the sample content to our own model which we previously created. To do so we click on change primary model and select the planning model we created in the TechEd folder in **My Files**.

![](/exercises/4_Story_Building/images/screenshot_add_01.png)

4. Now we add Measures and Dimensions to the rows and columns of the table. We add "Transaction Currency" to the rows of the table. 
This can be done by clicking on "Add Dimensions" and then we choose "Transaction Currency".

![](/exercises/4_Story_Building/images/screenshot03.png)

5. Next, we add the Time dimension to the columns of the table

6. For Liquidity Item we change the Filter:
select "Cash Closing", "Cash Opening" and "Cash Flows related to operating activities" and press "OK".

![](/exercises/4_Story_Building/images/screenshot05.png)

7. For better readability, we want the Transaction Currency column to be displayed as the first row of the table. 
This can be changed by dragging and dropping the Transaction Currency field in the Builder panel as the first row of the Rows section.

![](/exercises/4_Story_Building/images/screenshot06.png)

8. We also filter the time dimension to 2020, 2021 and 2022 (using "Add Filters" and "Time (Member)")  and expand the years 2020 and 2021. Let's also drill down on the liquidity items to have a more detailed view on the data. 

![](/exercises/4_Story_Building/images/screenshot07.png)

9. Save your story in between.

![](/exercises/4_Story_Building/images/4_SaveStory.png)

10. We now delete the 2022 data from the table (our actuals stop in December 2021, the data with zeroes is due to a data quality problem). For this we fold the different items in the table. Then we select the values in the column 2022 and hit the delete key. The final result should look like below. 

![](/exercises/4_Story_Building/images/screenshotdelete.png)

11. For better contrast in the story, we can change the background color of the table to white in the Styling panel.

![](/exercises/4_Story_Building/images/screenshot08.png)


## Exercise 4.2 Create the second table

Now that we have created our table with liquidity items, we also want to get insights into our influencer data. For that, we create another table below.

1. The rows of this table consist of "Transaction Currency", "Liquidity Item", "Company Code". "Liquidity Item" is filtered on "Influencers".
2. The columns consist of the measure "Amount", "Version" and "Time". 
3. We set the Time Hierarchy to "Year, Month", filter Time to "2021" and "2022" and set the background color to white again.

![](/exercises/4_Story_Building/images/screenshot09.png)

4. To directly see the exact liquidity item node, we can change the hierarchy on "Liquidity Item". We right click on the respective column, choose "Select Hierarchy" and click on "Show only leaves in widget". 

![](/exercises/4_Story_Building/images/screenshot10.png)
![](/exercises/4_Story_Building/images/screenshot11.png)

This way, we can directly see the liquidity item, without having to drill down the hierarchy.

![](/exercises/4_Story_Building/images/screenshot12.png)

5. Now, please save your story again.
![](/exercises/4_Story_Building/images/4_SaveStory.png)

## Summary

We have now created two tables in the story based on the imported data!
We can now continue to - [Exercise 5 - Create a Smart Predict Scenario](../5_Create_A_Smart_Predict_Scenario/README.md). 
If prompted whether to publish youd data changes, select "Leave" and do not publish your changes.

