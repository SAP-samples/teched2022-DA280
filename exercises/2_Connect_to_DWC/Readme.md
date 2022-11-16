# Exercise 2 - Connect to SAP Datawarehouse Cloud's Analytical Dataset

In this short exercise, we will create a connection from SAP Analytics Cloud to connect to the Analytical Dataset we created in our first exercise.

1. First, let us navigate to SAP Analytics Cloud and open the Connections panel: 
<br>![](/exercises/2_Connect_to_DWC/images/01_Connections.png)

2. SAP Data Warehouse Cloud offers a public OData API (details https://api.sap.com/api/ODataAPI/overview) to support the replication of models to SAP Analytics Cloud. Let us therefore add a connection and select the OData connection type:  
<br>![](/exercises/2_Connect_to_DWC/images/02_OData.png)

3. Last but not least, we need to configure the details:

If your SAP Analytics Cloud URL includes **EU10** (e.g. https://academy-t-sac.eu10.hcs.cloud.sap/):
- Connection Name: DA280_<your_sac_user_id>
- Data Service URL: https://academy-t-dwc.eu10.hcs.cloud.sap/api/v1/dwc/consumption/relational/<your_dwc_space_id>/<your_analytical_dataset> 
- Authentication Type: OAuth 2.0 Authorization Code
- OAuth Client ID: sb-d6553ac5-f665-49c6-8ad8-6ca2475ffba0!b130523|client!b3650
- Secret: bf2c0794-1eb0-4ae2-bf8b-f00a1abd7805$glUM5UWsx4lHGcpBEHmICF6JP4xqhv_4mYtiT9wrqCA=
- Token URL: https://academy-t-dwc.authentication.eu10.hana.ondemand.com/oauth/token 
- Authorization URL: https://academy-t-dwc.authentication.eu10.hana.ondemand.com/oauth/authorize

An example for the Data Service URL would be: https://academy-t-dwc.eu10.hcs.cloud.sap/api/v1/dwc/consumption/relational/TECHED_DEMO/V_Union_Actuals_and_Influencer  
<br>
<br>
If your SAP Analytics Cloud URL includes **US10** (e.g. https://academy-t-sac.us10.hcs.cloud.sap/):
- Connection Name: DA280_<your_sac_user_id>
- Data Service URL: https://academy-t-dwc.us10.hcs.cloud.sap/api/v1/dwc/consumption/relational/<your_dwc_space_id>/<your_analytical_dataset> 
- Authentication Type: OAuth 2.0 Authorization Code
- OAuth Client ID: sb-26782ba9-1e24-4a70-ba59-51713a91ac5a!b65895|client!b655
- Secret: d309d6b7-1514-40cb-9518-dfbc2ddcca7f$NN4Mpm18BE0nVEof9UMy5ofF5xUazwJnVY7OMe0xloQ=
- Token URL: https://academy-t-dwc.authentication.us10.hana.ondemand.com/oauth/token 
- Authorization URL: https://academy-t-dwc.authentication.us10.hana.ondemand.com/oauth/authorize

An example for the Data Service URL would be: https://academy-t-dwc.us10.hcs.cloud.sap/api/v1/dwc/consumption/relational/TECHED_DEMO/V_Union_Actuals_and_Influencer 
<br>
<br>

If your SAP Analytics Cloud URL includes **AP11** (e.g.https://academy-t-sac.ap11.hcs.cloud.sap/):
- Connection Name: DA280_<your_sac_user_id>
- Data Service URL: https://academy-t-dwc.ap11.hcs.cloud.sap/api/v1/dwc/consumption/relational/<your_dwc_space_id>/<your_analytical_dataset> 
- Authentication Type: OAuth 2.0 Authorization Code
- OAuth Client ID: sb-623ccfb1-8e5f-4c33-a10b-939703e77848!b853|client!b23
- Secret: bbf8384b-cd9e-4f7a-9958-2a54b2254de7$z3TuigvJ7ExsOr4Fk1kFn-GHCzdUPO7BwbTKR4rSuEk=
- Token URL: https://academy-t-dwc.authentication.ap11.hana.ondemand.com/oauth/token 
- Authorization URL: https://academy-t-dwc.authentication.ap11.hana.ondemand.com/oauth/authorize

An example for the Data Service URL would be: https://academy-t-dwc.ap11.hcs.cloud.sap/api/v1/dwc/consumption/relational/TECHED_DEMO/V_Union_Actuals_and_Influencer 

<br>![](/exercises/2_Connect_to_DWC/images/03_Configuration.JPG)

Finally, click on Create and you should receive a positive confirmation. Afterwards, you can move on to [Exercise 3 - Copy planning model and load data](/exercises/3_Copy_Model_and_Import_Data/).
