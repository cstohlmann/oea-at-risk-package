# Student Support Package: Predicting Chronic Absenteeism 

The Predicting Chronic Absenteeism package in Open Education Analytics (OEA) provides a set of technical assets to support a university or school system in developing a predictive model of students in their system who may become chronically absent and the most likely reason why they are becoming chronically absent in order to provide guidance for pro-active interventions to prevent or reduce high levels of absences. This OEA Package was developed through a partnership between Microsoft Education, Kwantum Analytics, and Fresno Unified School District in Fresno, California.

The <em>[OEA Chronic Absenteeism Package - Use Case Documentation](https://github.com/cstohlmann/oea-at-risk-package/blob/main/Chronic_Absenteeism/docs/OEA%20Chronic%20Absenteeism%20Package%20-%20Use%20Case%20Documentation.pdf)</em> provides guidance on the end-to-end process of developing a successful Chronic Absenteeism use case project, including how to engage stakeholders in the project, prior research on the use case problem domain and theory, how to map data sources to the theory of the problem, and how to implement principals of responsible data and AI in the process of predictive modelling.

This package can use several [OEA Modules](https://github.com/microsoft/OpenEduAnalytics/tree/main/modules) to help ingest data sources that are typically used to understand patterns of chronic absenteeism (see below for list of relevant OEA modules).  

## Problem Statement

Chronic absenteeism is generally defined as a student missing 10% or more of instructional time in school. Student absenteeism is a fundamental challenge to education systems, and it permeates education policy and practice discussions even more as result of the global pandemic. Machine learning offers the potential to find patterns of absenteeism across student demographic, attendance, engagement, achievement, and social-emotional measures to predict students at risk of becoming chronically absent so that proactive and preventative interventions can be utilized to support students.  

Education systems are responsible for addressing student absenteeism and can use a predictive model to focus resources to more precisely support students who are on a trajectory leading to chronic absenteeism, identify the best interventions to prevent absenteeism, and ultimately reduce absenteeism.  

## Use-Case Direction and Data-Type Requirements

The full Use-Case documentation for Predicting Chronic Absenteeism is [here](https://github.com/cstohlmann/oea-at-risk-package/blob/main/Chronic_Absenteeism/docs/OEA%20Chronic%20Absenteeism%20Package%20-%20Use%20Case%20Documentation.pdf). This document provides prior research on Chronic Absenteeism and a description of the process and decision-making for developing this use case in a way that demonstrates Microsoft’s Principles of Responsible Data and AI. It is highly recommended this document be reviewed by any education system considering using this package, and that the documentation be revised to the specific data and decisions for that system’s context. 

The predictive model provided in this OEA package combines several data sources identified through prior research to be strongly related to absenteeism: 
 - detailed student data, 
 - student patterns of academic digital engagement (both inside and outside school),
 - demographic data, 
 - academic data, 
 - school level data, and 
 - behavior data.
 
 ### Dashboard Outcomes
 This data was combined to provided insights into:

![alt text](https://github.com/cstohlmann/oea-at-risk-package/blob/main/Chronic_Absenteeism/docs/images/Chronic%20Absenteeism%20Dashboard%20Overview.png)
 <p align="center">
 <em>
 (Patterns of absenteeism by school, grade, geographic location, absence reason, and over time) 
 </em>
 </p>
 
![alt text](https://github.com/cstohlmann/oea-at-risk-package/blob/main/Chronic_Absenteeism/docs/images/Chronic%20Absenteeism%20Drivers%20Dashboard.png)
  <p align="center">
 <em>
 (A predictive model of potentially chronically absent students, that identifies the most likely reason (i.e. Drivers) why a student is predicted to become chronically absent) 
 </em>
 </p>

![alt text](https://github.com/cstohlmann/oea-at-risk-package/blob/main/Chronic_Absenteeism/docs/images/Chronic%20Absenteeism%20Social%20Worker%20Dashboard.png)
 <p align="center">
 <em>
 (A school-level dashboard for school support staff to quickly identify which students are at risk of becoming chronically absent, and for what reasons) 
 </em>
 </p>

![alt text](https://github.com/cstohlmann/oea-at-risk-package/blob/main/Chronic_Absenteeism/docs/images/Chronic%20Absenteeism%20Student%20Profile%20Dashboard.png)
 <p align="center">
 <em>
 (A student snapshot to provide real-time data to school and support staff) 
 </em>
 </p>

## Package Results/Solutions
The "Predicting Chronic Absenteeism" Use-Case from OEA can be used by system or institutional leaders, school, or department leaders, support staff, and educators to:
 - More accurately identify which students are at risk of becoming chronically absent or may move to a higher tier of absence
 - More quickly understand what type of support resources or interventions might be most appropriate to prevent or reduce absenteeism with individual students
 - Provide a real-time and detailed snapshot of students who are at risk of higher level of absence to school support staff to guide their decisions and actions based on engagement, academic, and well-being patterns of that student.

## Package Components
This Predicting Chronic Absenteeism package was developed by [Kwantum Analytics](https://www.kwantumanalytics.com/) in partnership with [Fresno Unified School District in California, USA](https://www.fresnounified.org/). The architecture and reference implementation for all modules is built on [Azure Synapse Analytics](https://azure.microsoft.com/en-us/services/synapse-analytics/) - with [Azure Data Lake Storage](https://docs.microsoft.com/en-us/azure/storage/blobs/data-lake-storage-introduction) as the storage backbone, and [Azure Active Directory](https://azure.microsoft.com/en-us/services/active-directory/) providing the role-based access control.

Assets in the Chronic Absenteeism use-case include:

1. [Data Dependencies](https://github.com/cstohlmann/oea-at-risk-package/tree/main/Chronic_Absenteeism/data_dependencies): For understanding the various schema mappings to OEA-standardized general-category tables (e.g. Activity tables), as well as the Caliper-adopted documentation within the tables.
2. [Documentation](https://github.com/cstohlmann/oea-at-risk-package/tree/main/Chronic_Absenteeism/docs): 
     * The <em>[OEA Chronic Absenteeism Package - Use Case Documentation](https://github.com/cstohlmann/oea-at-risk-package/blob/main/Chronic_Absenteeism/docs/OEA%20Chronic%20Absenteeism%20Package%20-%20Use%20Case%20Documentation.pdf)</em> provides guidance on the end-to-end process of developing a successful use case project, including how to engage stakeholders in the project, prior research on the use case problem domain and theory, how to map data sources to the theory of the problem, and how to implement principals of responsible data and AI in the process of predictive modelling.
     * For ingesting data from multiple sources, such as OEA modules into the data lake.
     * At some point: Guide to developing a predictive ML model of chronically absent students with Azure Machine Learning.
3. [Notebooks](https://github.com/cstohlmann/oea-at-risk-package/tree/main/Chronic_Absenteeism/notebooks): For cleaning, processing, anonymizing/pseudonymizing, and curating data within the data warehouse.
4. [Pipelines](https://github.com/cstohlmann/oea-at-risk-package/tree/main/Chronic_Absenteeism/pipelines): For an overarching picture of the processes used to create/train the machine learning model, and push respective data points to the dashboard template(s).
5. [PowerBI templates](https://github.com/cstohlmann/oea-at-risk-package/tree/main/Chronic_Absenteeism/powerbi): For exploring, visualizing, and deriving insights from the data.

### Overview of Module Dependencies for Package
This package can use existing OEA modules:

| Dependency | Description |
| --- | --- |
| [Ed-Fi Data Standards](https://github.com/microsoft/OpenEduAnalytics/tree/main/modules/Education_Data_Standards/Ed-Fi) | For typical SIS or MIS data, including detailed student attendance data, demographic data, and academic data. |
| Microsoft digital engagement data | Such as Teams [Education Insights Premium](https://github.com/microsoft/OpenEduAnalytics/tree/main/modules/Microsoft_Data/Microsoft_Education_Insights_Premium), or [Microsoft Graph](https://github.com/microsoft/OpenEduAnalytics/tree/main/modules/Microsoft_Data/Microsoft_Graph) data; digital activity/engagement data. |
| [Clever data](https://github.com/microsoft/OpenEduAnalytics/tree/main/modules/Digital_Learning_Apps_and_Platforms/Clever) | For additional activity data from other education applications. |
| [iReady data](https://github.com/microsoft/OpenEduAnalytics/tree/main/modules/Digital_Learning_Apps_and_Platforms/iReady) | For language and math (summative) assessments, if iReady applications are used in your education system. |

These OEA modules can be replaced with other types of data, and combined with other sources of data that the school or system has access to.

# Legal Notices
Microsoft and any contributors grant you a license to the Microsoft documentation and other content in this repository under the [Creative Commons Attribution 4.0 International Public License](https://creativecommons.org/licenses/by/4.0/legalcode), see the [LICENSE](https://github.com/microsoft/OpenEduAnalytics/blob/main/LICENSE) file, and grant you a license to any code in the repository under the [MIT License](https://opensource.org/licenses/MIT), see the [LICENSE-CODE](https://github.com/microsoft/OpenEduAnalytics/blob/main/LICENSE-CODE) file.

Microsoft, Windows, Microsoft Azure and/or other Microsoft products and services referenced in the documentation may be either trademarks or registered trademarks of Microsoft in the United States and/or other countries. The licenses for this project do not grant you rights to use any Microsoft names, logos, or trademarks. Microsoft's general trademark guidelines can be found at http://go.microsoft.com/fwlink/?LinkID=254653.

Privacy information can be found at https://privacy.microsoft.com/en-us/

Microsoft and any contributors reserve all other rights, whether under their respective copyrights, patents, or trademarks, whether by implication, estoppel or otherwise.

