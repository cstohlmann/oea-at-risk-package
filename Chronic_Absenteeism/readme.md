# At-Risk Package Use-Case: Predicting Chronic Absenteeism 

The Predicting Chronic Absenteeism package in Open Education Analytics (OEA) provides a set of technical assets to support a university or school system in developing a predictive model of students in their system who may become chronically absent, in order to provide pro-active interventions to prevent or reduce high levels of absences. This OEA Package was developed through a partnership between Microsoft Education, Kwantum Analytics, and Fresno Unified School District in Fresno, California.   

This package can use several [OEA Modules](https://github.com/microsoft/OpenEduAnalytics/tree/main/modules) to help ingest data sources that are typically used to understand patterns of chronic absenteeism (see below for list of relevant OEA modules).  

Chronic absenteeism is generally defined as a student missing 10% or more of instructional time in school. Student absenteeism is a fundamental challenge to education systems, and it permeates education policy and practice discussions even more as result of the global pandemic. Machine learning offers the potential to find patterns of absenteeism across student demographic, attendance, engagement, achievement, and social-emotional measures to predict students at risk of becoming chronically absent so that proactive and preventative interventions can be utilized to support students.  

Education systems are responsible for addressing student absenteeism and can use a predictive model to focus resources to more precisely support students who are on a trajectory leading to chronic absenteeism, identify the best interventions to prevent absenteeism, and ultimately reduce absenteeism.  

The full Use Case documentation for Predicting Chronic Absenteeism is here <strong><em>[ADD HYPERLINK]</strong></em>. This document provides prior research on Chronic Absenteeism and a description of the process and decision-making for developing this use case in a way that demonstrates Microsoft’s Principles of Responsible Data and AI. It is highly recommended this document be reviewed by any education system considering using this package, and that the documentation be revised to the specific data and decisions for that system’s context. 

The predictive model provided in this OEA package combines several data sources identified through prior research to be strongly related to absenteeism: 
 - detailed student data, 
 - student patterns of academic digital engagement (both inside and outside school),
 - demographic data, 
 - academic data, 
 - school level data, and 
 - behavior data.
 
 This data was combined to provided insights into:
  - Patterns of absenteeism by school, grade, geographic location, absence reason, and over time: <strong><em>[CONSIDER RE-PHRASING]</strong></em>
 <p align="center">
 <strong><em>
 [INCLUDE DASHBOARD PIC]
 </strong></em>
 </p>
 
  - A predictive model of potentially chronically absent students, that identifies the most likely reason (i.e. Drivers) why a student is predicted to become chronically absent:
<p align="center">
 <strong><em>
 [INCLUDE DASHBOARD PIC]
 </strong></em>
 </p>
 
  - A school-level dashboard for school support staff to quickly identify which students are at risk of becoming chronically absent, and for what reasons:
<p align="center">
 <strong><em>
 [INCLUDE DASHBOARD PIC]
 </strong></em>
 </p>
 
  - A student snapshot to provide real-time data to school and support staff:
 <p align="center">
 <strong><em>
 [INCLUDE DASHBOARD PIC]
 </strong></em>
 </p>

## Package Impact/Solutions
The "Predicting Chronic Absenteeism" package (Use-Case??) from OEA can be used by system or institutional leaders, school, or department leaders, support staff, and educators to:
 - More accurately identify which students are at risk of becoming chronically absent or may move to a higher tier of absence
 - More quickly understand what type of support resources or interventions might be most appropriate to prevent or reduce absenteeism with individual students
 - Provide a real-time and detailed snapshot of students who are at risk of higher level of absence to school support staff to guide their decisions and actions based on engagement, academic, and well-being patterns of that student.

## Package Components
The architecture and reference implementation for all technical assets for this package are built on Azure Synapse Analytics <strong><em>\[INCLUDE HYPERLINK\]</strong></em> - with Azure Data Lake Storage <strong><em>\[INCLUDE HYPERLINK\]</strong></em> as the storage backbone, and Azure Active Directory <strong><em>\[INCLUDE HYPERLINK\]</strong></em> providing the role-based access control.

Assets in the Chronic Absenteeism package (use-case??) include:

1. Documentation for ingesting data from  multiple sources, such as OEA modules into the data lake.
2. Notebooks for cleaning, transforming, anonymizing, and enriching data into the data warehouse.
3. Guide to developing a predictive ML model of chronically absent students using Azure Machine Learning.
4. PowerBI templates for exploring, visualizing, and deriving insights from the data.

## Package Overview of Module Dependencies
This package can use existing OEA modules:

1. [Ed-Fi Data Standards](https://github.com/microsoft/OpenEduAnalytics/tree/main/modules/Education_Data_Standards/Ed-Fi) for typical SIS or MIS data, including detailed student attendance data, demographic data, and academic data.
2. Microsoft digital engagement data, such as Teams [Education Insights Premium](https://github.com/microsoft/OpenEduAnalytics/tree/main/modules/Microsoft_Data/Microsoft_Education_Insights_Premium) or [Microsoft Graph](https://github.com/microsoft/OpenEduAnalytics/tree/main/modules/Microsoft_Data/Microsoft_Graph) data.
3. [Clever data](https://github.com/microsoft/OpenEduAnalytics/tree/main/modules/Digital_Learning_Apps_and_Platforms/Clever) for additional activity data from other education applications.
4. [iReady data](https://github.com/microsoft/OpenEduAnalytics/tree/main/modules/Digital_Learning_Apps_and_Platforms/iReady) for language and math (summative) assessments, if iReady applications are used in your education system.

These OEA modules can be replaced with other types of data, and combined with other sources of data that the school or system has access to.

## Package setup \[TO BE ADDED\]
1. 
## Package components
Out-of-the box assets for this OEA package include: 
1. [Data Dependencies](): 
2. [Pipelines](): x pipeline templates - 
3. [Notebooks](): x notebooks - 
4. [PowerBI Template](): 

  <p align="center">
  <em> <strong>[INSERT SAMPLE PICTURE OF PACKAGE DASHBOARD TEMPLATE]</em> </strong>
 </p>
 
 <p align="center">
  <em>(This dashboard example represents only data from - LIST MODULES USED HERE.)</em>
 </p>

The Chronic Absenteeism package [welcomes contributions](https://github.com/microsoft/OpenEduAnalytics/blob/main/CONTRIBUTING.md). 

This module was developed by [Kwantum Analytics](https://www.kwantumanalytics.com/) in partnership with [Fresno Unified School District]() \[SHOULD I INCLUDE THIS WITH A LINK?\]. The architecture and reference implementation for all modules is built on [Azure Synapse Analytics](https://azure.microsoft.com/en-us/services/synapse-analytics/) - with [Azure Data Lake Storage](https://docs.microsoft.com/en-us/azure/storage/blobs/data-lake-storage-introduction) as the storage backbone, and [Azure Active Directory](https://azure.microsoft.com/en-us/services/active-directory/) providing the role-based access control.
### For more info on modules used
\[TO BE COMPLETED\]

| Resource | Description |
| --- | --- |
| [Education Insights Premium Module](https://github.com/microsoft/OpenEduAnalytics/tree/main/modules/Microsoft_Data/Microsoft_Education_Insights_Premium) | Module used and referenced when building out this use-case template. |
| [iReady Module](https://github.com/microsoft/OpenEduAnalytics/tree/main/modules/Digital_Learning_Apps_and_Platforms/iReady) | Module used and referenced when building out this use-case template. |
|  |  |
|  |  |
|  |  |
|  |  |

# Legal Notices
Microsoft and any contributors grant you a license to the Microsoft documentation and other content in this repository under the [Creative Commons Attribution 4.0 International Public License](https://creativecommons.org/licenses/by/4.0/legalcode), see the [LICENSE](https://github.com/microsoft/OpenEduAnalytics/blob/main/LICENSE) file, and grant you a license to any code in the repository under the [MIT License](https://opensource.org/licenses/MIT), see the [LICENSE-CODE](https://github.com/microsoft/OpenEduAnalytics/blob/main/LICENSE-CODE) file.

Microsoft, Windows, Microsoft Azure and/or other Microsoft products and services referenced in the documentation may be either trademarks or registered trademarks of Microsoft in the United States and/or other countries. The licenses for this project do not grant you rights to use any Microsoft names, logos, or trademarks. Microsoft's general trademark guidelines can be found at http://go.microsoft.com/fwlink/?LinkID=254653.

Privacy information can be found at https://privacy.microsoft.com/en-us/

Microsoft and any contributors reserve all other rights, whether under their respective copyrights, patents, or trademarks, whether by implication, estoppel or otherwise.

