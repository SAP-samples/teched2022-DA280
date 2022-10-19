# Exercise 1 - Acquiring Data from SAP Data Warehouse Cloud

In this exercise, we first look for external data on energy prices in the Data Marketplace of SAP Data Warehouse Cloud. We will then combine this data with our internal cash flow statement actuals and create a consumable view. Finally, we create a connection from SAP Analytics Cloud to SAP Data Warehouse Cloud that will allow us to easily transfer the data into a planning model. 

## Exercise 1.1 Adding External Data via Data Marketplace

After completing these steps you will have acquired energy external data from Data Markeplace into your space.

1. First, let us navigate to the Data Marketplace. As the name suggests, it is like a marketplace for data consumers and data providers, and allows the easy integration of external data. If this is news to you, feel free to explore the various data products that are available. 
<br>![](/exercises/ex1/images/01-DM.png)

2. Let us now search for a data product that contains the historic evolution of the energy price, as well as a forecast into the future. Thus, type in "2022_TechEd_DA280" into the search field. We will find exactly one data product that matches our search. 
<br>![](/exercises/ex1/images/02-Search.png)

3. Select the data product and read through its description. Notice that it has various categories assigned (which improve its visibility in the search)  and is accessible for free.
<br>![](/exercises/ex1/images/03-Description.png)

4. Load the data product into your DWC space. To do so, select the top-right button "Load for Free", select the respective space in the pop-up and load the data product.
<br>![](/exercises/ex1/images/04-Load.png)

5. It will now take a moment until the external data is accessible in our space. Luckily, DWC notifies us when the table replication is completed successfully. Once done, let us navigate to the Data Builder and select the newly created remote table with business name "V_Energy_Prices_TechEd_Demo". If it looks like the following, you successfully completed our first exercise (yeay!). 
<br>![](/exercises/ex1/images/05-Preview.png)


## Exercise 1.2 Combining external and internal data

After completing these steps you will have created an Analytical Dataset in SAP Data Warehouse Cloud, which combines external data from Data Marketplace with internal actuals. 

1. Now that we have acquired the external data and made it accessible in our space, let us now combine it with our internal data. To do so, let us create a new graphical view and **union** "V_Energy_Prices_TechEd_Demo" with our actuals data in "T_S4_ACT". 

First, drag and drop the "T_S4_ACT" table into the canvas. Afterwards, select the "V_Energy_Prices_TechEd_Demo" table from the leftside panel and hover it over the first table on the canvas. DWC will suggest you three options (union, join or replace), from which you will select the first one.

Note that DWC is intelligent and already mapped all columns from the first table to those columns from the second table with the same business name. Only for the "version" column, you will need to manually map both sides. 

The result should look like the following: 
<br>![](/exercises/ex1/images/06-Join.png)

2. Finally, let us navigate to the output node and define the view properties. Let us adapt the following: 

  - Business_Name: "V Union Actuals and Influencer"
  - Semantic Usage: "Analytical Dataset"
  - Expose for Consumption: Enabled
  - Measures: "Amount"
  - Attribues: All remaining columns 

Note: The OData API for SAP Data Warehouse Cloud only provides access to DWC artefacts which are exposed for consumption. This is why it is important to enable this field. 

<br>![](/exercises/ex1/images/07-ADS.png)

3. One last action: Let us deploy the Analytical Dataset. 

## Exercise 1.2 Connect SAC to DWC

After completing these steps you will have...



## Summary

You've now ...

Continue to - [Exercise 2 - Exercise 2 Description](../ex2/README.md)

