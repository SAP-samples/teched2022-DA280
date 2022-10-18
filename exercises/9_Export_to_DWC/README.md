# 9 - Export to DWC
We now want to export the generated plan data from SAP Analytics Cloud to SAP Data Warehouse Cloud. The plan data could be used for downstream processing and combined plan vs. ACT reporting there. 

## 9.1 - OAuth Client in SAP Analytics Cloud
An OAuth Client has already been set up in SAP Analytics Cloud. You need its credentials and the SAC system's authorization URL and Token URL.

Navigate to System - Administration. 
<br>![](/exercises/9_Export_to_DWC/images/8_1.png)

Go to App Integration and take note of the Authorization URL and the Token URL. Then open the "SACtoDWC" OAuth client.
<br>![](/exercises/9_Export_to_DWC/images/8_2.png)

Take note of the OAuth client ID and secret.
<br>![](/exercises/9_Export_to_DWC/images/8_3.png)

In SAP Data Warehouse Cloud, go to Connections and click 'Create'.
<br>![](/exercises/9_Export_to_DWC/images/8_4.png)

Choose conenction type 'Cloud Data Integration'.
<br>![](/exercises/9_Export_to_DWC/images/8_5.png)

Under connection details, enter the URL for the Data Export Service. In our case: https://my-sac-tenant.eu10.sapanalytics.cloud/api/v1/dataexport/administration
Also, add the OAuth token endpoint URL that you get from the App Integration page in SAP Analytics Cloud.
<br>![](/exercises/9_Export_to_DWC/images/8_6.png)

Enter the OAuth Client ID and its secret.
<br>![](/exercises/9_Export_to_DWC/images/8_7.png)

In the next step, provide a name for the connection. 
<br>![](/exercises/9_Export_to_DWC/images/8_8.png)

