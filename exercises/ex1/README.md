# Exercise 1 - Acquiring Data from SAP Data Warehouse Cloud

In this exercise, we first look for external data on energy prices in the Data Marketplace of SAP Data Warehouse Cloud. We will then combine this data with our internal cash flow statement actuals and create a consumable view. Finally, we create a connection from SAP Analytics Cloud to SAP Data Warehouse Cloud that will allow us to easily transfer the data into a planning model. 

## Exercise 1.1 Adding External Data via Data Marketplace

After completing these steps you will have created an Analytical Dataset in SAP Data Warehouse Cloud, which combines external data from Data Marketplace with internal actuals. 

1. First, let us navigate to the Data Marketplace. As the name suggests, it is like a marketplace for data consumers and data providers, and allows the easy integration of external data. If this is news to you, feel free to explore the various data products that are available. 
<br>![](/exercises/ex1/images/01-DM.png)

2. Let us now search for a data product that contains the historic evolution of the energy price, as well as a forecast into the future. Thus, type in "2022_TechEd_DA280" into the search field. We will find exactly one data product that matches our search. 
<br>![](/exercises/ex1/images/02-Search.png)

3. Select the data product and read through its description. Notice that it has various categories assigned (which improve its visibility in the search)  and is accessible for free.
<br>![](/exercises/ex1/images/03-Description.png)

4. Load the data product into your DWC space. To do so, select the top-right button "Load for Free", select the respective space in the pop-up and load the data product.
<br>![](/exercises/ex1/images/04-Load.png)

5. It will now take a moment until the external data is accessible in our space. Luckily, DWC notifies us when the table replication is completed successfully. Once done, let us navigate to the Data Builder and select the newly created remote table with business name "
V_Energy_Prices_TechEd_Demo". It should look like the following: 
<br>![](/exercises/ex1/images/05-Preview.png)

7. Finally, let us now have a look into the external data we acquired. We therefore navigate to the Data Builder


## Exercise 1.2 Connect SAC to DWC

After completing these steps you will have...



## Summary

You've now ...

Continue to - [Exercise 2 - Exercise 2 Description](../ex2/README.md)

