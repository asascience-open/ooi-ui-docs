#![](http://www.rpsgroup.com/images/2012-specific/RPSlogo.aspx) OOI Web UI Construction 
# QA/QC Data Evaluation

| Use Case ID | 018 |
| --- | --- |
| Name | QA/QC Data Evaluation                 |
| Scope of Work | Status UI |
| Actors: | PSs |
| Requester | OL |
| Description: | It permits authorized users (PSs) to view a data set, determine scientific quality, make changes to improve the data, flag data, annotate the data. |


##Need Statement

Data require periodic examination and adjustment by SMEs. Flaws in processing, unrealistic instrument errors, or communication drops all need to be checked and appropriately flagged.

##Definition

The SME downloads a data set and performs QC with a mixture of experience, other data sets and analysis. They then add any corrected values, modify metadata if needed and annotate the data or data set if necessary. They then upload the new data to the OOI.

##Assumptions 

- HITL efforts will utilize OOI SMEs with read/write privileges to particular data sets.
- HITL efforts will 'add' data corrections' and not delete the original data.
- The SME will use their own analysis tools on their local machine


##Scenario
An RSN scientist is reviewing data and discovers errors that need to be corrected.

STEPS:

1. The scientist downloads a data set to their local machine.
2. Using their own tools, examines that data and makes necessary modifications to the data values.
3. During this process the scientist makes some annotations to individual data value cells.
4. When finished, the "HITL editor" tool (available only to authorized SMEs) prompts the scientist to enter metadata explaining what was changed and why.
5. After the scientist finishes with the metadata updates and clicks "finish", the HITL tool creates a new data structure that incorporates the SME corrected data values and annotations.
6. The scientist uploads the corrected data set where the OOI system assimilates the changes
