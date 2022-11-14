# Exercise 2 - Connect to SAP Datawarehouse Cloud's Analytical Dataset

In this short exercise, we will create a connection from SAP Analytics Cloud to connect to the Analytical Dataset we created in our first exercise.

1. First, let us navigate to the SAP Analytics Cloud and open the Connections panel: 
<br>![](/exercises/2_Connect_to_DWC/images/01_Connections.png)

2. SAP Data Warehouse Cloud offers a public OData API (details https://api.sap.com/api/ODataAPI/overview) to support the replication of models to SAP Analytics Cloud. Let us therefore add a connection and select the OData connection type:  
<br>![](/exercises/2_Connect_to_DWC/images/02_OData.png)

3. Last but not least, we need to configure the details:

If your tenant URL includes EU10:
- Connection Name: DA280_<your_sac_user_id>
- Data Service URL: https://academy-t-dwc.eu10.hcs.cloud.sap/api/v1/dwc/consumption/relational/<your_dwc_space_id>/<your_analytical_dataset> 
- Authentication Type: OAuth 2.0 Authorization Code
- OAuth Client ID: sb-7eea113e-4f71-48ae-9699-16cd0de3020b!b130334|client!b3650
- Secret: 6cdd9c60-ae89-41e8-86e8-c2f53a8df5e4$kvBO_DATme4Y-poz6diWwKeU7_RA2wFLJLEswncgc5E=
- Token URL: https://academy-t-dwc.authentication.eu10.hana.ondemand.com/oauth/token 
- Authorization URL: https://academy-t-dwc.authentication.eu10.hana.ondemand.com/oauth/authorize

An example for the Data Service URL would be: https://academy-t-dwc.eu10.hcs.cloud.sap/api/v1/dwc/consumption/relational/TECHED_DEMO/V_Union_Actuals_and_Influencer  

If your tenant URL includes US10:
- Connection Name: DA280_<your_sac_user_id>
- Data Service URL: https://academy-t-dwc.us10.hcs.cloud.sap/api/v1/dwc/consumption/relational/<your_dwc_space_id>/<your_analytical_dataset> 
- Authentication Type: OAuth 2.0 Authorization Code
- OAuth Client ID: sb-7eea113e-4f71-48ae-9699-16cd0de3020b!b130334|client!b3650
- Secret: 6cdd9c60-ae89-41e8-86e8-c2f53a8df5e4$kvBO_DATme4Y-poz6diWwKeU7_RA2wFLJLEswncgc5E=
- Token URL: https://academy-t-dwc.authentication.us10.hana.ondemand.com/oauth/token 
- Authorization URL: https://academy-t-dwc.authentication.us10.hana.ondemand.com/oauth/authorize

An example for the Data Service URL would be: https://academy-t-dwc.us10.hcs.cloud.sap/api/v1/dwc/consumption/relational/TECHED_DEMO/V_Union_Actuals_and_Influencer 

If your tenant URL includes AP11:
- Connection Name: DA280_<your_sac_user_id>
- Data Service URL: https://academy-t-dwc.ap11.hcs.cloud.sap/api/v1/dwc/consumption/relational/<your_dwc_space_id>/<your_analytical_dataset> 
- Authentication Type: OAuth 2.0 Authorization Code
- OAuth Client ID: sb-7eea113e-4f71-48ae-9699-16cd0de3020b!b130334|client!b3650
- Secret: 6cdd9c60-ae89-41e8-86e8-c2f53a8df5e4$kvBO_DATme4Y-poz6diWwKeU7_RA2wFLJLEswncgc5E=
- Token URL: https://academy-t-dwc.authentication.ap11.hana.ondemand.com/oauth/token 
- Authorization URL: https://academy-t-dwc.authentication.ap11.hana.ondemand.com/oauth/authorize

An example for the Data Service URL would be: https://academy-t-dwc.ap11.hcs.cloud.sap/api/v1/dwc/consumption/relational/TECHED_DEMO/V_Union_Actuals_and_Influencer 

<br>![](/exercises/2_Connect_to_DWC/images/03_Configuration.png)

Finally, click on Create and you should receive a positive confirmation.
