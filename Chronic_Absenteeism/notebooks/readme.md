# Package Notebooks
Given the current state of the At-Risk package and Chronic Absenteeism use-case, this use-case includes a single class notebook: <em>ChronicAbsenteeism_py.ipynb</em>. This class notebook currently contains 3 functions:
 - <strong>curate_fromStage2p:</strong> Parent function that commands subsequent functions to run if analysis is to be done on the Education Insights module data as a source of activity data.
     * <strong>process_activity_stage2p_data:</strong> Schema transformation and creation of the tables outlined in the [data_dependencies](https://github.com/cstohlmann/oea-at-risk-package/tree/main/Chronic_Absenteeism/data_dependencies) section of this use-case.
     * <strong>write_activity_stage3p_data:</strong>: Without re-pseudonymization (for sake of tracability of keys), the code takes the activity tables and writes them to stage 3p.

### Additional Notes:
 - This notebook will likely become obsolete within the next few months, as schema transformation is expected to take place at the module level. However, this use-case is expected to contain several other notebooks responsible for data aggregation and cleaning.
