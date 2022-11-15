# 9 - Export to DWC
We now want to export the generated plan data from SAP Analytics Cloud to SAP Data Warehouse Cloud. The plan data could be used for downstream processing and combined plan vs. ACT reporting there. 

## 9.1 - OAuth Client in SAP Analytics Cloud
An OAuth Client has already been set up in SAP Analytics Cloud. You need its credentials and the SAC system's authorization URL and Token URL. Since you are not authorized to go to System - Administration - App Integration (where you would usually find this), please use the following credentials and URLs:

If your SAP Analytics Cloud URL includes EU10:
<br>OAuth Client ID: sb-25518ec4-4cc5-444f-883b-97ce341a9e18!b130365|client!b3650
<br>Secret: cccfdbbc-9a90-4bc8-9c4e-2b8d50102bf6$xzsl5LGQNwvZIst2jqotcNOd-CEq7d8reWDWFeFebQY=
<br>Token URL: https://academy-t-sac.authentication.eu10.hana.ondemand.com/oauth/token
<br>Authorization URL: https://academy-t-sac.authentication.eu10.hana.ondemand.com/oauth/authorize

If your SAP Analytics Cloud URL includes US10:
<br>OAuth Client ID: sb-25518ec4-4cc5-444f-883b-97ce341a9e18!b130365|client!b3650
<br>Secret: cccfdbbc-9a90-4bc8-9c4e-2b8d50102bf6$xzsl5LGQNwvZIst2jqotcNOd-CEq7d8reWDWFeFebQY=
<br>Token URL: https://academy-t-sac.authentication.us10.hana.ondemand.com/oauth/token
<br>Authorization URL: https://academy-t-sac.authentication.us10.hana.ondemand.com/oauth/authorize

If your SAP Analytics Cloud URL includes AP11:
<br>OAuth Client ID: sb-25518ec4-4cc5-444f-883b-97ce341a9e18!b130365|client!b3650
<br>Secret: cccfdbbc-9a90-4bc8-9c4e-2b8d50102bf6$xzsl5LGQNwvZIst2jqotcNOd-CEq7d8reWDWFeFebQY=
<br>Token URL: https://academy-t-sac.authentication.ap11.hana.ondemand.com/oauth/token
<br>Authorization URL: https://academy-t-sac.authentication.ap11.hana.ondemand.com/oauth/authorize

In SAP Data Warehouse Cloud, go to Connections and click 'Create'.
<br>![](/exercises/9_Export_to_DWC/images/8_4.png)

Choose conenction type 'Cloud Data Integration'.
<br>![](/exercises/9_Export_to_DWC/images/8_5.png)

Under connection details, enter the URL for the Data Export Service. In our case: https://my-sac-tenant.eu10.sapanalytics.cloud/api/v1/dataexport/administration
Also, add the OAuth token endpoint URL that you get from the App Integration page in SAP Analytics Cloud.
<br>![](/exercises/9_Export_to_DWC/images/8_6.png)

Enter the OAuth Client ID and its secret.
<br>![](/exercises/9_Export_to_DWC/images/8_7.png)

In the next step, provide a name for the connection and create it. 
<br>![](/exercises/9_Export_to_DWC/images/8_8.png)

Now, navigate to the Data Builder (you remember that from our first exercises) and create a new Data Flow.
<br>![](/exercises/9_Export_to_DWC/images/8_9.png)

In the panel on the left hand side, go to sources and open the newly created connection. Navigate to the SAC namespace.
<br>![](/exercises/9_Export_to_DWC/images/8_10.png)

You receive a list of all available models on the connected SAP Analytics Cloud tenant. Go back to your model in SAP Analytics Cloud and copy the model ID from its URL.
<br>![](/exercises/9_Export_to_DWC/images/8_11.png)

You can search for the model back in the Data Flow and then drag the fact data on to the canvas.
<br>![](/exercises/9_Export_to_DWC/images/8_12.png)

The Data Flow must write the data into a table. Add a table.
<br>![](/exercises/9_Export_to_DWC/images/8_13.png)

Give the table a name and click 'Create and Deploy Table'
<br>![](/exercises/9_Export_to_DWC/images/8_14.png)

Afterwards, name the Data Flow and Deploy it. Afterwards, click 'Save'.
<br>![](/exercises/9_Export_to_DWC/images/8_15.png)
<br>![](/exercises/9_Export_to_DWC/images/8_16.png)

Now you can run the Data Flow. Once you run it, you can jump to the Data Integration Monitor.
<br>![](/exercises/9_Export_to_DWC/images/8_17.png)

Refreh the status ocassionaly in the monitor until the Data Flow run is completed after a few moments.
<br>![](/exercises/9_Export_to_DWC/images/8_18.png)

Go back to the Data Flow, mark the table and toggle the data preview.

<br>![](/exercises/9_Export_to_DWC/images/8_19.png)

**Congratulations! You have completed all exercises! Thanks so much!**
