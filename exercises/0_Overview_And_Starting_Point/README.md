# 0 - Overview

In this exercise, you will learn about the high-level architecture of the artefacts used in this workshop and the connection between them. 
Also, you will learn about the pre-configured elements that have been prepared by SAP to facilitate the workshop. 
Lastly, you can find a short introduction about the most important involed product functionalities. 

## 0.1 - Architecture
<br>![](/exercises/0_Overview_And_Starting_Point/images/TechEd2022_Architecture.png)

This workshop takes place in SAP Data Warehouse Cloud and SAP Analytics Cloud. First of all, internal data is combined with external data from the Data Marketplace. Afterwards, a connection to SAP Analytics Cloud is set up using the DWC Public Consumption API. After loading the data from the previously created union to SAP Analytics Cloud, a story in SAP Analytics Cloud is enriched with the respective tables for data entry and simulation before we then create the needed objects like the predictive scenario, multi actions and data actions. After running the prediction and saving the results into a planning version, we set up a connection and load data to SAP Data Warehouse Cloud using the Data Export Service offered by SAP Analytics Cloud. 

## 0.2 - SAP Data Warehouse Cloud - Data Builder and S/4 Actual Data
<br>![](/exercises/0_Overview_And_Starting_Point/images/0.2_DataBuilder.png)

In the Data Builder of SAP Data Warehouse Cloud, you can define data models for your data with a technical, model-driven approach in the graphical tools or in the powerful SQL editor of the data layer. Two Data Builder artefacts have been pre-created for this workshop.

- A table containing cash flow statement actuals from S/4HANA
- A view on top of this table

## 0.3 SAP Data Warehouse Cloud - Data Marketplace
Data Marketplace is fully integrated into SAP Data Warehouse Cloud. It’s tailored for businesses to easily integrate third-party data. You can search and purchase analytical data from data providers. The data comes in form of objects packaged as data products that can be used in one or several spaces of your SAP Data Warehouse Cloud tenant.

Data products are either provided for free or require the purchase of a license at a certain cost. Some data products are available as one-time shipments, other data products are regularly updated by data providers.

To get data products into your SAP Data Warehouse Cloud tenant and consume them, you can follow a simple workflow:

<br>![](/exercises/0_Overview_And_Starting_Point/images/0.3_DataMarketplace.png)

## 0.4 Bi-directional Integration for Planning
SAP Data Warehouse Cloud and SAP Analytics Cloud are better together. This is why SAP delivered the bi-directional integration between SAP Data Warehouse Cloud and SAP Analytics Cloud for planning. This enables you to load fact data and master data from Data Warehouse Cloud to SAP Analytics Cloud. Similarly, you can seamlessly retract fact data, master data, and audit data from SAP Analytics Cloud models and use it in SAP Data Warehouse Cloud.

Most importantly, this enables you to use actual data from SAP Data Warehouse Cloud in your planning tables in SAP Analytics Cloud. Additionally, you can join plan and actual data from multiple sources in common views in SAP Data Warehouse Cloud that you can then use for live reporting or any other kind of downstream processing of your plan data. You can also meet corporate requirements to store all steering-relevant data in one data warehouse as a single source of truth.

It is important to understand that the use case of bi-directional integration between SAP Analytics Cloud and SAP Data Warehouse Cloud is enabled by two public APIs:

- SAP Data Warehouse Cloud provides a public OData API (Controlled Release with wave 11) to pull data from DWC and integrate it into SAP Analytics Cloud using the OData Services Connection.
- SAP Analytics Cloud provides the Data Export Service (DES) API (generally available with QRC2.2022) to pull data from SAC and make it available in Data Warehouse Cloud using remote tables or data flows.

The following image already gives a good high-level overview of our scenario:

<br>![](/exercises/0_Overview_And_Starting_Point/images/0.4_Bidirectional_Integration.png)
