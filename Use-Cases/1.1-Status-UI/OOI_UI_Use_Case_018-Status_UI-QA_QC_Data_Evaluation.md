#![](http://www.rpsgroup.com/images/2012-specific/RPSlogo.aspx) OOI Web UI Construction 
# QA/QC Data Evaluation

| Use Case ID | 018 |
| --- | --- |
| Name | QA/QC Data Evaluation                 |
| Scope of Work | Status UI |
| Actors: | Facility Operator, Data Manager |
| Requester | OL |
| Description: | It permits authorized users to view a data set, determine scientific quality, flag data of questionable data quality, annotate the data. |


##Need Statement

Data require periodic examination by the Data management team. Flaws in processing, unrealistic values, or trend changes consistent with biofouling problems  is identified and then appropriately flagged.

##Definition

The Data evaluator uses the u-Frame system tools which apply automated Qa/Qc algorithms to enable Qa/Qc check of OOI data.  The data evalautor utilizes quick look plots to further assess data quality.  The evaluator flags and antonates any data of questionable quality and informs the data manager of the status.  

##Assumptions 



##Scenario
An data evaluator is reviewing data and assessing it quality.

STEPS:

1. The evaluator logs into uframe, and selects a specific data product of interest
2. The data in the uFrame system has applied automated algorithms for Qa/Qc
3. The evaluator then utilizes the quick look plot to examine the data
4. The data evaluator identifies some data of questionable quality and applies appropiate flags
5. The data evaluator then annotate the concerns
6. The data evaluator then informs the data manager 
7. The data manager can then initate a "deep" dive into the flagged data
