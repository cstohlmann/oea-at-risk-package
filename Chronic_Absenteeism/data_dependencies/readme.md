# Data Dependencies

## Module/Data Source Dependencies
For this Chronic Absenteeism Package, it is built using (3 or 4) table types, using (2 or 3) OEA modules out-of-the-box:
1. Attendance Data (e.g. SIS Module)
2. SIS Data (e.g. SIS Module)
3. Activity Data (e.g. Microsoft Education Insights Module)
4. Behavior Data (e.g. ) <strong> \[MIGHT REMOVE\] </strong>

## Notes and Planning for v1.0 Activity Relationship Table:

### Standing Questions:
 - Can we write all these tables to Delta instead of the unstructured format of JSON?

### First-Draft Concepts:
<em> Currently, thinking of using 3 first-draft relationship tables </em> 
1. Event Class/Table <strong>(USING THIS ONE)</strong>:

     Current idea is to use this as basic, fast first iteration. Column assignments/details:
```
    1. id - (column SignalID from Insights Activity table)
    2. type - ToolUseEvent class... [MAPS TO TABLE 2 BELOW]
    3. actor - (column AadId from Insights Roster table|column ActorId from Insights Activity table)
    4. action - Used
    5. object - SoftwareApp class (AppNames column from Insights Activity table)
    6. eventTime - TimeStamp Type
    7. generated - AggregateMeasures class... [MAPS TO TABLE 4 BELOW]
    8. edApp - (thinking might use column AppName from Insights Activity table; if we create a single SoftwareApp item, being "Insights")
```
2. SoftwareApplication Class/Table <strong>(USING THIS ONE)</strong>:

```
    1. type ("Term" Type) - 
    2. host (String Type) - 
    3. ipAddress (String Type) - 
    4. userAgent (String Type) - 
    5. version (String Type) - (column schemaVersion from Insights Activity table)
```

3. ToolUseEvent Table <strong>(IGNORE THIS TABLE FOR NOW)</strong>:

```
    1. Event - ToolUseEvent
    2. Actor - StudentId
    3. Action - Used
    4. Object - SoftwareApplication
    5. Generated - AggregateMeasureCollection
```
4. AggregateMeasure Class/Table <strong>(USING THIS ONE)</strong>

```
    1. type
    2. metricValue - (column meetingDuration from Insights Activity table)
```
5. Action Class/Table <strong>(TO BE ADDED IN FUTURE DRAFTS??)</strong>

    <em><strong>[TO BE ADDED]</em></strong>
    
    Intention would be to add this additional table to discern the various SignalTypes from various Apps (making the data served to PowerBI more granular).
    

### References:
| Resource | Description |
| --- | --- |
| [ToolUseEvent Table](https://www.imsglobal.org/spec/caliper/v1p2#ToolUseEvent) | Information and specs on ToolUseEvent table. |
| [Event Class/Table](https://www.imsglobal.org/spec/caliper/v1p2#Event) | Information and specs on Event class. |
| [SoftwareApplication Class/Table](https://www.imsglobal.org/spec/caliper/v1p2#softwareapplication) | Information and specs on SoftwareApplication class. |
| [AggregationMeasure Class/Table](https://www.imsglobal.org/spec/caliper/v1p2#AggregateMeasureCollection ) | Information and specs on Aggregation Measure |

