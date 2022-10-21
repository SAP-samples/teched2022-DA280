# DA280 - Build an Integrated Planning Scenario with Data and Analytics Solutions

## Description

This repository contains the material for the SAP TechEd 2022 session called DA280 - Build an Integrated Planning Scenario with Data and Analytics Solutions.  

## Overview

In this session, we will build an end-to-end integrated planning application with SAP Data Warehouse Cloud and SAP Analytics Cloud using the bi-directional data transfer between the two solutions. Besides the data transfer, the session covers data modeling, including the data marketplace in SAP Data Warehouse Cloud, as well as the creation of a planning model with predictive analytics and the respective front end for data entry.


## Use Case
Energy prices are increasing continuously. Companies are worried about the direct impact on their results and cash flow. Therefore, we want to create an automated liquidity forecast with SAP Analytics Cloud's predictive analytics capabilities on top of internal financial and external data from SAP Data Warehouse Cloud. 

To do so, we look for external data on energy prices in the Data Marketplace within SAP Data Warehouse Cloud. We add this data to our internal cash flow statement actuals and load it to SAP Analytics Cloud to serve as the basis for our new liquidity forecast.


## Requirements

The requirements to follow the exercises in this repository are:

- SAP SAC tenant

- SAP DWC tenant

The above requirements have already been met and have been pre-created by SAP. Apart from that, we recommend basic proficiency with modeling and story building in SAP Analytics Cloud and basic proficiency with SAP Data Warehouse Cloud. However, the exercises are suitable for everyone if the materials recommended in the 'Learn More' section are considered.

Exercise 0 explains the architecture of the exercises and provides information regarding each of the components. It is strongly recommended content but does not include hands-on exercises.

The hands-on exercises begin with Exercise 1.

## Exercises

Provide the exercise content here directly in README.md using [markdown](https://guides.github.com/features/mastering-markdown/) and linking to the specific exercise pages, below is an example.

- [Exercise 0 Overview and Starting Point](exercises/0_Overview_And_Starting_Point/)
- [Exercise 1 - Acquiring Data from SAP Data Warehouse Cloud](exercises/1_DataMarketplace/README.md/)
- [Exercise 2 - Connect to DWC](exercises/2_Connect_to_DWC/Readme.md/)


  
**OR** Link to the Tutorial Navigator for example...

Start the exercises [here](https://developers.sap.com/tutorials/abap-environment-trial-onboarding.html).

**IMPORTANT**

Your repo must contain the .reuse and LICENSES folder and the License section below. DO NOT REMOVE the section or folders/files. Also, remove all unused template assets(images, folders, etc) from the exercises folder. 

## Learn More
To learn more about SAP Analytics Cloud, refer to the following sources of information:
- https://open.sap.com/courses/sac4
- 	https://open.sap.com/courses/sac5 

To learn more about SAP Data Warehouse Cloud, refer to the following sources of information:
- https://developers.sap.com/mission.data-warehouse-cloud-get-started.html 
- https://community.sap.com/topics/data-warehouse-cloud/getting-started

To learn more about the bi-directional integration between SAP Analytics Cloud and SAP Data Warehouse Cloud for planning, refer to these sources of information:
- [Blog post: Introducing the Bi-Directional Integration of SAP Data Warehouse Cloud and SAP Analytics Cloud for Planning](https://blogs.sap.com/2022/06/21/introducing-the-bi-directional-integration-of-sap-data-warehouse-cloud-and-sap-analytics-cloud-for-planning/?preview_id=1561485)
- [Devtoberfest session](https://groups.community.sap.com/t5/devtoberfest/bi-directional-integration-between-sap-data-warehouse-cloud-and/ec-p/9392#M52)

## How to obtain support

Support for the content in this repository is available during the actual time of the online session for which this content has been designed. Otherwise, you may request support via the [Issues](../../issues) tab.

## License
Copyright (c) 2022 SAP SE or an SAP affiliate company. All rights reserved. This project is licensed under the Apache Software License, version 2.0 except as noted otherwise in the [LICENSE](LICENSES/Apache-2.0.txt) file.
