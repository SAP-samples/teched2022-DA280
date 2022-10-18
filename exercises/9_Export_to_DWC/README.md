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

In SAP Data Warehouse Cloud, 
