# OEA At-Risk Package

This OEA At-Risk Package <em><strong>(suite??)</em></strong> contains solutions to a variety of different scenarios, when assessing whether a student is "at-risk". From a pedagogical standpoint, "at-risk" is defined as students that are on the verge of being at-risk for academic struggle or failure. OEA has worked to identify the following three primary at-risk categories in which, <em><strong>(schools/insutitutions??)</em></strong> seek solutions towards:

<strong><em>[INSERT IMAGE OF AT-RISK FLOW CHART]</em></strong>

With this package <em><strong>(suite??)</em></strong>, the <em><strong>(predictions/outcomes/results??)</em></strong> can be used to identify and test <em><strong>(teacher/social-worker??)</em></strong> methods of intervention to better support and uphold student success.

## Framework for At-Risk Package Use-Cases

### Library of Use-Cases:

The table below characterizes and categorizes the various use-cases that can be addressed through the OEA At-Risk package. The assets within each of the use-cases can be used to provide answers <em><strong>(and predictions??)</em></strong> to school and <em><strong>(district/partnership??) [Note: Supposedly, Australia's name for school districts are "partnerships", which is why I included it here]</em></strong> leaders. 

| Academic At-Risk | Chronic Absenteeism | Vulnerable Student |
| --- | --- | --- |
| Predicting students at risk of failing a class, course, or semester | Predicting students at different levels of absenteeism, and identifying most likely reasons for absenteeism to guide preventative actions | Predicting students who are or may become vulnerable outside of school and need additional school or state supports |
| Predicting students at risk of a graduation or not completing a degree program |

### Data Requirements (and OEA modules):

The table below specifies stage 2 data <em><strong>(expected??)</em></strong> requirements that are considered <em><strong>(in theory or practice??)</em></strong> for the OEA At-Risk package.

<strong><em>Note: The assets provided within each of these use-case templates are general solutions. This means that they lean on specific modules out-of-the-box, but can be customized to incorporate the use of other modules or data sources.</em></strong>

| Academic At-Risk | Chronic Absenteeism | Vulnerable Student |
| --- | --- | --- |
| SIS Data: School, department, course/class rosters, class subject, grade level, race/ethnicity, other demographics | SIS Data: School, department, course/class rosters, class subject, grade level, race/ethnicity, other demographics | SIS Data: School, department, course/class rosters, class subject, grade level, race/ethnicity, other demographics |
| School climate and teacher behaviors (e.g. substitutes) | School climate and teacher behaviors (e.g. substitutes) | School climate and teacher behaviors (e.g. substitutes) |
| LMS Data (assignment grades, assignment engagement) |  LMS data (assignment grades, assignment engagement) |  |
| Platform \& App signals (Clever, MS Graph, Edu Insights, iReady) | Platform \& App signals (Clever, MS Graph, Edu Insights, iReady) |  |
| Social-emotional learning \& competencies data |  | Social-emotional learning \& competencies data | 
| Online sentiment analysis |  | <strong><em>(Online??)</strong></em> Sentiment analysis |
|  | Social network data (if feasible) |  |
|  | Behavior data |  |
|  | Absence and absence code data |  |
|  | Health, Medical, and Disabilities data | Health, Medical, and Disabilities data |
|  | Transportation and school-move data |  |
|  | Safety and Justice system data |  |
|  |  | Reflect data (Insights) |

## How to Navigate the Use-Case Templates

Currently, this package contains 3 primary use-cases (academic at-risk, chronic absenteeism, and student vulnerability) and 7 assets per use-case, which can be found in the following sub-folder directory.

<strong><em>[CONSIDER INSERTING AN IMAGE OF CHRONIC ABSENTEEISM SUB-DIRECTORY PARTITIONING]</em></strong>

 - <strong>Machine Learning (ML) Models:</strong> Contains various <strong><em>(checkpoints of versioning??)</strong></em> for the machine learning models trained.
      * <em>Note: These are often subject to changes and updates as more discovery becomes available, and model-training experimentation is conducted. </em>
 - <strong>Data Dependencies:</strong> Lists the schema mappings from module data tables to the OEA-defined, general-category tables.
      * <em>e.g. MS Education Insights Premium Module Activity table -> OEA-defined Events, SoftwareApplications, and AggregrateMeasure tables.</em>
 - <strong>Documentation:</strong> Explanation of how to tailor the use-case assets to <strong><em>(school/institution-specific??)</strong></em> needs.
 - <strong>Notebooks:</strong> Set of all notebooks for processing and enriching used in the implementation of the use-case (.ipynb files). 
      * <em>e.g. Data aggregation, data manipulation, simple analysis operations, and schema transformation. </em>
 - <strong>Pipelines:</strong> Set of all pipeline templates used in the implementation of the use-case (.zip folders).
      * <em>Note: These often rely on notebooks, thus ensure that all use-case-relevant notebooks are imported.</em>
 - <strong>Power BI Templates:</strong> Set of all Power BI dashboard templates for relaying results and value from data analysis (.pbix files).
 - <strong>Rubrics:</strong> Use-case-specific OEA rubrics, that outline functionality and current state of the assets within the use-case.


