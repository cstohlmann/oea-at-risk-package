# Documentation

## Use Case Documentation

The [OEA Chronic Absenteeism Package - Use Case Documentation](https://github.com/cstohlmann/oea-at-risk-package/blob/d52b29fa918a95c6cb084e70f54a9a6aa2cdf00e/Chronic_Absenteeism/docs/OEA%20Chronic%20Abs%20Package%20-%20Use%20Case%20Doc.pdf) provides guidance on the end-to-end process of developing a successful Chronic Absenteeism use case project. This document includes 
 - defining of the use case problem,
 - stakeholder identification and engagement in the project,
 - mapping research theory to data,
 - and implementing principles of responsible data and AI in the process of predictive modelling. 
The use case document was completed in collaboration with through a partnership between Microsoft Education, [Kwantum Analytics](https://www.kwantumanalytics.com/), and [Fresno Unified School District](https://www.fresnounified.org/) in Fresno, California.

## First Draft of Explanation and "How to tailor this package"

Maria comment: This needs to include SIS data as those are the MAIN data sources for attendance as outcome feature to be predicted. This whole section needs to outline the relationship between features as a research problem, doesn't it?

This "Predicting Chronic Absenteeism" package currently leans on the [Education Insights Module](https://github.com/microsoft/OpenEduAnalytics/tree/main/modules/Microsoft_Data/Microsoft_Education_Insights_Premium) for activity data. In order to leverage a different activity-based module or data source,
1. <strong>Class Notebook Editing:</strong> First, refer to the class notebook (ChronicAbsenteeism_py). The methods outlining curation of the Insights activity table maps to 3 different OEA-standard tables (i.e. Event, SoftwareApplication, and AggregateMeasure).
      * <em>What needs to be done:</em> you will need to create a schema mapping to these three tables from your activity data/table.
2. <strong>Pipeline Review:</strong> Next, refer to the main pipeline within this package. 
      * <em>What needs to be done:</em> This will need to be updated to account for your tenant name, and storage account names, along with any other additional customizations made to data-source dependencies (e.g. updating the pipeline activities to curate Graph activity data versus Insights activity data).
3. <strong>Model Training and Development:</strong> This package currently relies on AutoML to conduct training of the machine learning model. This is used to develop the predictive algorithm for identfying potential instances of chronic absenteeism.
      * <em>What needs to be done:</em> If you prefer to hand-build a model, you can go into the pipeline and rather than kicking off the data to AutoML, build your own notebook for model training and development. You can view model training progress and iterations in the <strong><em>(AutoML Studio??)</strong></em>
      * <strong><em>[INCLUDE ANY ADDITIONAL INFORMATION AS CHAD SEES FIT]</strong></em>
4. <strong>PowerBI Updates:</strong> If the table names, column names or schemas are changed from any original names to new names; these will need to be reflected in the Power BI dashboard template.
      * <em>What needs to be done:</em> If the above is applicable to you, make the necessary updates to the dashboard to mirror the schema changes. Also, ensure that you've made adjustments to graphs and visualizations to reflect solution(s) to your personal problem statement(s).
