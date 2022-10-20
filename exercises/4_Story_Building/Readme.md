

# Exercise 4 - Story Building
Now that we have imported the data from DWC to our SAC planning model, we can start building a table on top.
For that, we go to Files, navigate to our TechEd folder and open the SAP__FI_CLM_LIQUIDITY_PLANNING Story.

On the first page, ...

Let's swtich to the second page to create the table.






## Exercise 4.1 Create the first table

After completing these steps you will have created...

1. To add a table to the story, we click on "Table" in the "Insert" toolbar.

![](/exercises/4_Story_Building/images/screenshot01.png)

2. We move the table to the left side of the story and resize its size as shown in the screenshot.

![](/exercises/4_Story_Building/images/screenshot02.png)


3. Now we add Measures and Dimensions to the rows and columns of the table. We start adding "Transaction Currency" to the rows of the table. 
This can be done by clicking on "Add Dimensions" and then we choose "Transaction Currency".

![](/exercises/4_Story_Building/images/screenshot03.png)

4. Next, we add the Time dimension to the columns of the table

5. For Measures we change the Filter:

![](/exercises/4_Story_Building/images/screenshot04.png)

select "Cash Closing", "Cash Opening" and "Cash Flows related to operating activities" and press "OK".

![](/exercises/4_Story_Building/images/screenshot05.png)

6. For better readability, we want the Transaction Currency column to be displayed as the first row of the table. 
This can be changed by drag and drop in the Builder panel.

![](/exercises/4_Story_Building/images/screenshot06.png)

7. We also filter the time dimension to 2020, 2021 and 2022 and expand the years 2020 and 2021. Let's also drill down on the liquidity items to have a more detailed view on the data. 

![](/exercises/4_Story_Building/images/screenshot07.png)

8. For better contrast in the story, we can change the background color of the table to white in the Styling panel.

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



## Summary

We have now created two tables in the story based on the imported data!
We can now continue to - [Exercise 5 - Create a Smart Predict Scenario](../ex5/README.md).

