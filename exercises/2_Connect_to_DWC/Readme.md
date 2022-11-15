# Exercise 2 - Connect to SAP Datawarehouse Cloud's Analytical Dataset

In this short exercise, we will create a connection from SAP Analytics Cloud to connect to the Analytical Dataset we created in our first exercise.

1. First, let us navigate to SAP Analytics Cloud and open the Connections panel: 
<br>![](/exercises/2_Connect_to_DWC/images/01_Connections.png)

2. SAP Data Warehouse Cloud offers a public OData API (details https://api.sap.com/api/ODataAPI/overview) to support the replication of models to SAP Analytics Cloud. Let us therefore add a connection and select the OData connection type:  
<br>![](/exercises/2_Connect_to_DWC/images/02_OData.png)

3. Last but not least, we need to configure the details:

If your SAP Analytics Cloud URL includes EU10:
- Connection Name: DA280_<your_sac_user_id>
- Data Service URL: https://academy-t-dwc.eu10.hcs.cloud.sap/api/v1/dwc/consumption/relational/<your_dwc_space_id>/<your_analytical_dataset> 
- Authentication Type: OAuth 2.0 Authorization Code
- OAuth Client ID: sb-d6553ac5-f665-49c6-8ad8-6ca2475ffba0!b130523|client!b3650
- Secret: bf2c0794-1eb0-4ae2-bf8b-f00a1abd7805$glUM5UWsx4lHGcpBEHmICF6JP4xqhv_4mYtiT9wrqCA=
- Token URL: https://academy-t-dwc.authentication.eu10.hana.ondemand.com/oauth/token 
- Authorization URL: https://academy-t-dwc.authentication.eu10.hana.ondemand.com/oauth/authorize

An example for the Data Service URL would be: https://academy-t-dwc.eu10.hcs.cloud.sap/api/v1/dwc/consumption/relational/TECHED_DEMO/V_Union_Actuals_and_Influencer  

If your SAP Analytics Cloud URL includes US10:
- Connection Name: DA280_<your_sac_user_id>
- Data Service URL: https://academy-t-dwc.us10.hcs.cloud.sap/api/v1/dwc/consumption/relational/<your_dwc_space_id>/<your_analytical_dataset> 
- Authentication Type: OAuth 2.0 Authorization Code
- OAuth Client ID: sb-c4c8f8d0-27e2-4dd8-a192-e38c5cc7e451!b65895|client!b655
- Secret: 911ecd68-342d-4c13-97a0-9cfdfb773829$qqEYbkQG5y1kYxz2VTHfmw5ysKUBmsNfVE0IiRAUzUc=
- Token URL: https://academy-t-dwc.authentication.us10.hana.ondemand.com/oauth/token 
- Authorization URL: https://academy-t-dwc.authentication.us10.hana.ondemand.com/oauth/authorize

An example for the Data Service URL would be: https://academy-t-dwc.us10.hcs.cloud.sap/api/v1/dwc/consumption/relational/TECHED_DEMO/V_Union_Actuals_and_Influencer 

If your SAP Analytics Cloud URL includes AP11:
- Connection Name: DA280_<your_sac_user_id>
- Data Service URL: https://academy-t-dwc.ap11.hcs.cloud.sap/api/v1/dwc/consumption/relational/<your_dwc_space_id>/<your_analytical_dataset> 
- Authentication Type: OAuth 2.0 Authorization Code
- OAuth Client ID: sb-b17faf8d-5dcb-4e74-b149-40028217a4e7!b853|client!b23
- Secret: e4bd4ea1-e1bc-4a8f-bd5b-056b61610323$bY-qioYrby5utXpXAP0xxG1fT7p5shRvKqN-02t3XE4=
- Token URL: https://academy-t-dwc.authentication.ap11.hana.ondemand.com/oauth/token 
- Authorization URL: https://academy-t-dwc.authentication.ap11.hana.ondemand.com/oauth/authorize

An example for the Data Service URL would be: https://academy-t-dwc.ap11.hcs.cloud.sap/api/v1/dwc/consumption/relational/TECHED_DEMO/V_Union_Actuals_and_Influencer 

<br>![](/exercises/2_Connect_to_DWC/images/03_Configuration.png)

Finally, click on Create and you should receive a positive confirmation.
