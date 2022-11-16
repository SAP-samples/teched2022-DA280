# Exercise 8 - Story Building & forecasting/planning
In this exercise, you will include the previously created Multi Action for Time Series Forecast and a Data Action for the Deletion Step into the built story.

## Add Data Action and Multi Action to the story

After completing these steps you will have knowledge of how to involve Data Actions and Multi Actions into a story using an action trigger event.

1. In this exercise, the "SAP__FI_CLM_LIQUIDITY_PLANNING" Story is used. This File can be found in the MyFiles folder copied from the "TechEd2022_DA280_SampleContent" as "TechEd2022_DA280_#Lastname" in the prior exercises.

![Exercise8_01](https://user-images.githubusercontent.com/112930664/202113235-af831d1b-ce88-4007-a411-52d6abc04fd5.png)

2. Navigate to page 2 in the navigation panel to include a Multi Action and a Data Action to the Story. In the beginning of this Task, the Story should look similar to the one in the image below.

![](/exercises/8_Story_Building_Forecasting_Planning/images/8_Story2.png)

3. At first, you will create the Multi Action Trigger event. Therefore, please press the + Button in the Insert Panel of the menu bar. When clicking the planning trigger, another window as shown in 4. will pop up to the screen. Make sure that you are in Edit mode.

![](/exercises/8_Story_Building_Forecasting_Planning/images/8_PlanningTrigger2.png)

4. The Predictive Forecast is created as a Multi Action, the delete operation is created as a Data Action Trigger. We will begin by adding the predictive forecast. Therefore please click the Multi Action Trigger button within the popup window.

![Exercise8_04](https://user-images.githubusercontent.com/112930664/202113242-aa140fc5-35f1-4e6f-9cb7-dffe75679c3a.png)

5. For including the prior created Multi Action into the Planning Trigger, you can add the underlying Multi Action through the Builder Panel. There you can also add a shown Label for the Multi Action Event Trigger. For the Multi Action, select the "Predictive Liquidity Forecast" you have created before as part of this TechEd Demo.

![](/exercises/8_Story_Building_Forecasting_Planning/images/8_MA.png)

6. To create the second Data Action Trigger, navigate to the Action Trigger Insertion similar to 3. & 4. but instead of choosing a Multi Action Trigger, this time we will add a Data Action Trigger instead. Similar to 5., we give that Data Action Trigger an underlying Data Action and a shown label to describe what happens after clicking it. The underlying Data Action is the one created in the prior exercise for Deletion. In Case of this Demo, we named it "Delete_Predictive_Forecast" + our last name.

![](/exercises/8_Story_Building_Forecasting_Planning/images/8_DA.png)

7. We fix the Target Version parameter to Predictive Forecast to always clear our Predictive Forecast Version.
![](/exercises/8_Story_Building_Forecasting_Planning/images/8_Parameter.png) 

8. After creating both the Multi Action Trigger and the Data Action Trigger events, our Canvas should look similar to the one below.

![](/exercises/8_Story_Building_Forecasting_Planning/images/8_Overview.png))

9. Finally, we can first run the Delete Data Action and then our Predictive Forecast Multi Action and review the results. For that, we need to add the Predictive Forecast to the version filter of the table and drill down to the energy expense line item (depending on if you had the Liquidity Item hierarchy active or not).

![](/exercises/8_Story_Building_Forecasting_Planning/images/8_DrillDown.png)

## Summary

Now that you have built in the prior created Action triggers, you have learnt how to include these into a story in SAC.

Continue to [Exercise 9 - Export to DWC](../9_Export_to_DWC/README.md)
