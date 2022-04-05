# Pipelines
This section of the use-case contains _ pipelines, including a main pipeline that curates and enriches the data while also pushing relevant data to Power BI to be visualized. 

This main pipeline <em>(i.e. ml_main_pipeline)</em> consists of 4 components:
1. <strong>Data Cleaning and Aggregation:</strong>

<p align="center">
  <img src="https://github.com/cstohlmann/oea-at-risk-package/blob/main/Chronic_Absenteeism/docs/images/Main%20Pipeline%20(pt.%201).png?raw=true" alt="Main Pipeline (pt. 1)"/>
</p>

<p align="center">
 <em>
 (Cleans and aggregates data tables) 
 </em>
 </p>

2. <strong>Join to Model Table:</strong>

<p align="center">
  <img src="https://github.com/cstohlmann/oea-at-risk-package/blob/main/Chronic_Absenteeism/docs/images/Main%20Pipeline%20(pt.%202).png?raw=true" alt="Main Pipeline (pt. 2)"/>
</p>

<p align="center">
 <em>
 (Takes unified/curated data tables and joins this to the machine learning model table) 
 </em>
 </p>
 
 3. <strong>AutoML Trigger:</strong>

<p align="center">
  <img src="https://github.com/cstohlmann/oea-at-risk-package/blob/main/Chronic_Absenteeism/docs/images/Main%20Pipeline%20(pt.%203).png?raw=true" alt="Main Pipeline (pt. 3)"/>
</p>

<p align="center">
 <em>
 (Triggers and pushes the table(s) to AutoML from Synapse to construct and train a machine learning model) 
 </em>
 </p>
 
  4. <strong>Serve to PowerBI:</strong>

<p align="center">
  <img src="https://github.com/cstohlmann/oea-at-risk-package/blob/main/Chronic_Absenteeism/docs/images/Main%20Pipeline%20(pt.%204).png?raw=true" alt="Main Pipeline (pt. 4)"/>
</p>

<p align="center">
 <em>
 (Retrieves the model trained from AutoML to and analyzes the over the data to be predicted - and then pushes analysis results to PowerBI) 
 </em>
 </p>
