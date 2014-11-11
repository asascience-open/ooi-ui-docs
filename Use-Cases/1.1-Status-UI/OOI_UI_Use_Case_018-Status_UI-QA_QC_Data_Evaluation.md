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

- Marine Implementing Organization (MIO) provides "lookup table" on which QC algorithms are applicable to which L1 and L2 data products. This lookup table also contains threshold or range values for each L1 and L2 data product. This table is ingested into the uFrame database and made available to the UI.

##Scenario
1) An data evaluator is reviewing data and assessing it quality.

STEPS:

1. The evaluator logs into User Interface, and selects a specific L1 data product of interest
2. The data in the uFrame system has applied automated QA/QC algorithms for this L1 data product. Therefore the User Interface provides two sets of data for this data product: L1A is the original data product, L1B is the data product with QA/QC applied.
3. The evaluator selects to view the L1B data product
4. The User Interface displays a quick look plot which also displays QC flags and threshold & range values used. Evaluator analyzes the data.
5. The data evaluator identifies some data of questionable quality and adds additional flags
6. The data evaluator then annotate the concerns
7. The data evaluator then informs the data manager 
8. The data manager can then initate a "deep" dive into the flagged data
