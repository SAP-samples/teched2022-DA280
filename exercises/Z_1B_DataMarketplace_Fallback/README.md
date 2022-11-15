This is a fallback exercise in case you could not load data from the Data Marketplace! Since you had issues loading the data from Data Marketplace, we are getting the data from the shared objects in the data builder. You will learn how to do this below - it is simple and has no negative implications on the further workshop flow. 

## Exercise 1.2 Combining data and creating a consumable view (fallback version)

In Exercise 1.2 you will create an Analytical Dataset in SAP Data Warehouse Cloud, which combines the energy price data with internal actuals. 

1. We create a new graphical view and **union** "V_Energy_Prices_TechEd_Demo" with our actuals data in "T_S4_ACT". 

- First, drag and drop the "T_S4_ACT" table into the canvas (the table is available under Shared Objects / Tables)
- Afterwards, select the "V_Energy_Prices_TechEd_Demo" table from the leftside panel and hover it over the first table on the canvas. DWC will suggest you three options (UNION, JOIN or REPLACE), from which you will select the first one (UNION).
- Note that DWC is smart and already mapped all columns from the first table to those columns from the second table with the same business name. You will need to manually map both sides only for the "version" column. 

The result should look like the following: 
<br>![](/exercises/1_DataMarketplace/images/1.2_Union_New.png)

2. Finally, let us navigate to the output node and define the view properties. Let us adapt the following: 

  - Business_Name: "V Union Actuals and Influencer"
  - Semantic Usage: "Analytical Dataset"
  - Expose for Consumption: Enabled
  - Measures: "Amount"
  - Attributes: All remaining columns 

Note: The OData API for SAP Data Warehouse Cloud only provides access to DWC artefacts which are exposed for consumption. This is why it is important to enable the field Expose for Consumption. 

<br>![](/exercises/1_DataMarketplace/images/1.2_Result.png)

3. One last action: Let us deploy the Analytical Dataset. 
<br>![](/exercises/1_DataMarketplace/images/08-Deploy.png)

You have now successfully created a consumable view in SAP Data Warehouse Cloud. Let us now navigate to SAP Analytics Cloud and continue with - [Exercise 2 - Connect to DWC](/exercises/2_Connect_to_DWC/)


