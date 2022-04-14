# OEA Student Support Packages

This collection of OEA Student Support Packages contains technical resources for a variety of common education use cases, related to predicting whether a student needs specialized support. Depending on their context, students may need academic support for specific skills or knowledge domains; they may need support to ensure they can attend and engage in school; or they may need support with their home, health, or safety context. The OEA community has identified three primary categories of student supports that are needed in both primary, secondary and post-secondary education systems. 

![alt text](https://github.com/cstohlmann/oea-at-risk-package/blob/main/images/studentSupportPackages.png)

The OEA packages in this collection can be used to set up the data resources, stakeholder engagement, responsible AI processes, machine learning models, and dashboards that can identify patterns of supports needed and predict which individual students are likely to become in need of supports. The predictions can help education systems and schools choose the right methods of intervention to reduce or prevent student challenges and better support each student’s success. 

Each use case package includes Use Case Documentation that provides guidance on the end-to-end process of developing a successful use case project, including how to engage stakeholders in the project, prior research on the use case problem domain and theory, how to map data sources to the theory of the problem, and how to implement principles of responsible data and AI in the process of predictive modelling. 

## Library of Student Support Use-Cases 

The table below describes the use-cases that can be addressed through the OEA Student Support packages.  

| [Chronic Absenteeism](https://github.com/cstohlmann/oea-at-risk-package/tree/main/Chronic_Absenteeism) | [Academic At-Risk](https://github.com/cstohlmann/oea-at-risk-package/tree/main/Academic_At_Risk) | [Vulnerable Student](https://github.com/cstohlmann/oea-at-risk-package/tree/main/Vulnerable_Students) |
| --- | --- | --- |
| Predicting students at different levels of absenteeism, and identifying most likely reasons for absenteeism to guide preventative actions | Predicting students at risk of failing a class, course, or semester; predicting students at risk of a not graduating or not completing a degree program |Predicting students who are or may become vulnerable outside of school and need additional school or state supports |

## Data Requirements (and OEA modules)

The table below outlines the type of data sources that are most often used to report and develop predictive models for each category of Student Supports. 

<strong><em>Note:  The assets provided within each of these use-case templates are general solutions. This means that they can use specific OEA modules, but they can also use other data sources that an education system or school has.</em></strong>

| [Chronic Absenteeism](https://github.com/cstohlmann/oea-at-risk-package/tree/main/Chronic_Absenteeism) | [Academic At-Risk](https://github.com/cstohlmann/oea-at-risk-package/tree/main/Academic_At_Risk) | [Vulnerable Student](https://github.com/cstohlmann/oea-at-risk-package/tree/main/Vulnerable_Students) |
| --- | --- | --- |
| SIS or MIS Data: Attendance, school, department, course rosters, class subject, grade level, student behavior, and demographics as needed | SIS or MIS Data: Attendance, school, department, course rosters, class subject, grade level, student behavior, and demographics as needed | SIS or MIS Data: Attendance, school, department, course rosters, class subject, grade level, student behavior, and demographics as needed |
| School climate or student well-being data | School climate or student well-being data | School climate or student well-being data | 
| LMS Data (assignment grades, assignment engagement, marks or grades) | LMS Data (assignment grades, assignment engagement, marks or grades) | LMS Data (assignment grades, assignment engagement, marks or grades) |
| Digital learning platform & app use data | Digital learning platform & app use data | Digital learning platform & app use data |
| Health, medical, and disabilities data | Health, medical, and disabilities data | Health, medical, and disabilities data |
| Transportation and school-move data | | |
| | | Safety and Justice system data |

## Package Assets

Currently, this package contains 3 primary packages (academic at-risk, chronic absenteeism, and student vulnerability) and 7 assets per package, which can be found in the following sub-folder directory.

![alt text](https://github.com/cstohlmann/oea-at-risk-package/blob/main/Chronic_Absenteeism/docs/images/Chronic%20Absenteeism%20Folder%20Partitioning.png)

 - <strong>Documentation:</strong> Each package includes Use Case Documentation that provides guidance on the end-to-end process of developing a successful use case project, including how to engage stakeholders in the project, prior research on the use case problem domain, and how to implement principles of responsible data and AI in practice. This folder also provides an explanation of how to tailor the use-case assets to the specific needs of an education system or school. 
 - <strong> Machine Learning (ML) Models:</strong>  Contains technical assets and methodological guidance for the machine learning models trained. 
      * <em> Note: These are often subject to changes and updates as more discovery becomes available, and model-training experimentation is conducted. </em>
 - <strong>Data Dependencies:</strong> Lists the schema mappings from module data tables to the OEA-defined, general-category tables. 
      * <em>MS Education Insights Premium Module Activity table -> OEA-defined Events, SoftwareApplications, and AggregrateMeasure tables. </em>
 - <strong>Notebooks:</strong> Set of all notebooks for processing and enriching data used in the implementation of the use-case (.ipynb files). 
      * <em>e.g. Data aggregation, data manipulation, simple analysis operations, and schema transformation. </em>
 - <strong>Pipelines:</strong> Set of all pipeline templates used in the implementation of the use-case (.zip folders).
      * <em>Note: These often rely on notebooks, thus ensure that all use-case-relevant notebooks are imported.</em>
 - <strong>Power BI Templates:</strong> Set of all Power BI dashboard templates for relaying results and value from data analysis (.pbix files).


