# Exercise 8 - Story Building & forecasting/planning
In this exercise, you will include the previously created Multi Action for Time Series Forecast and a Data Action for the Deletion Step into the built story.

## Add Data Action and Multi Action to the story

After completing these steps you will have knowledge of how to involve Data Actions and Multi Actions into a story using an action trigger event.

1. In this exercise, the "SAP__FI_CLM_LIQUIDITY_PLANNING" Story is used. This File can be found in the MyFiles folder copied from the "TechEd2022_DA280_SampleContent" as "TechEd2022_DA280_#Lastname" in the prior exercises.

//Image 8_01 missing

2. Navigate to page 2 in the navigation panel to include a Multi Action and a Data Action to the Story. In the beginning of this Task, the Story should look similar to the one in the image below.
//Image 8_02 missing

3. At first, you will create the Multi Action Trigger event. Therefore, please press the + Button in the Insert Panel of the menu bar. When clicking the planning trigger, another window as shown in 4. will pop up to the screen.
//Image 8_03

4. The Predictive Forecast is created as a Multi Action, the delete operation is created as a Data Action Trigger. We will begin by adding the predictive forecast. Therefore please click the Multi Action Trigger button within the popup window.

//Image 8_04

5. For including the prior created Multi Action into the Event Trigger, you can add the underlying Multi Action through the Builder Panel. There you can also add a shown Label for the Multi Action Event Trigger. For the Multi Action, select the "Predictive Liquidity Forecast" you have created before as part of this TechEd Demo.

//Image 8_06

6. To create the second Data Action Trigger, navigate to the Action Trigger Insertion similar to 3. & 4. but instead of choosing a Multi Action Trigger, this time we will add a Data Action Trigger instead.


![Ex8_1](https://user-images.githubusercontent.com/112930664/197132153-11371e97-0ce1-403f-9528-cc845b7d1217.png)
2.	Navigate to page 2 in the navigation panel to create another story for the predictive forecast. After including the multi action trigger and the data action trigger, the story should look similar to the one below.
![ex8_2](https://user-images.githubusercontent.com/112930664/197132155-2f714d97-e6c3-4f5e-b771-7b51a3c2089a.png)
3. At first, we are creating a Multi Action Trigger event. Therefore we press the + Button above and navigate to Planning Trigger. When clicking the Planning Trigger, another window as shown in 4. will pop up.
![ex8_3](https://user-images.githubusercontent.com/112930664/197132158-d7b919f0-38a4-4597-8d91-89933381e1c3.png)
4. The predictive forecast is created as a multi action, the delete operation is created as a data Action Trigger. At first, we will add the predictive forecast. Therefore please click the Multi Action Trigger button within the popup window. 
![ex8_4](https://user-images.githubusercontent.com/112930664/197132160-4979846c-f3fa-40ef-9d57-f69ff7c9dceb.png)
5. For the Multi Action Trigger, you can add the underlying Multi Action through the Builder panel. There you can also add a shown Label.
For the multi action, select the SAP__FI_CLM_PLF_RUN_PRED_LIQ_FC_FOR_PRIVATE_VERSION.
![ex8_5](https://user-images.githubusercontent.com/112930664/197132148-c9f94641-211a-46b8-9a21-dae29a3ba2c3.png)
6. To create the second Data Action Trigger, navigate to the Action Trigger insertion similar to 3. & 4. but instead of the Multi Action Trigger, this time we will add a Data Action Trigger.
![ex8_6](https://user-images.githubusercontent.com/112930664/197132150-d1e7e66d-5b82-48f0-a18e-8b052a55aefd.png)
7. Similar to 5., we give the Data Action Trigger an underlying Data Action and a shown Label. In this case, we select the SAP__FI_CLM_LIQPLN_DEL_VERSION as the underlying Data Action. Further below within the builder panel, you also have the option to change parameters, so you could for example set the version to change to a fixed value, so you always use this Action Trigger only for the chosen Value. 
![ex8_7](https://user-images.githubusercontent.com/112930664/197132151-98ed35c9-e6c3-4f99-94ad-4f07047f12b7.png)
## Summary

Now that you have built in the prior created Action triggers, you have learnt how to include these into a story in SAC.

Continue to [Exercise 9 - Export to DWC](../9_Export_to_DWC/README.md)
