#![](http://www.rpsgroup.com/images/2012-specific/RPSlogo.aspx) OOI Web UI Construction 
#Update Metadata in a Data Product

| Use Case ID | 032 |
| --- | --- |
| Name | Update Metadata in a Data Product |
| Scope of Work | Status UI |
| Actors: | Marine Operator, Science, Data manager, Data Ealuator|
| Requester | OL |
| Description: | Updaterequired metadata fields when a data product is produced|


##Definition

OOI Data Products must have associated metadata which explains data provenance, associated information provided by the marine during ship deployments, commercial vendor sensor calibration files.

##Assumptions :

- The OOI Metadata Model has been created and baselined.
- The OOI Metadata Model includes metadata fields that meet the needs ocean science community.
- A metadata database has been created 
- The schema of the metadata database accommodates all metadata in the OOI Metadata Model

##Scenario

The following steps describe how the operator or project scientist will update the metadata.


1. A Data Product Algorithm has been updated with new calibration data provided by a sensor vendor. 
  1. A new calibration file has been provided by the commericial vendor for a particular sensor to the Marine Operator
  2. The Marine IO uploads the file into OOInet.  
  3. The Marine IO navigates to the senor and links the calibration file to the appropiate sensor
  4. The uFrame database stores the new calibration values

2. When the new calibration is applied to the OOINet system, the uFrame database will update all data product metadata values which have changed. Data product metadata shall include:
  1. Name of and link to the Data Product Specification document
  2. name of and link to the Data Product Algorithm code
  3. Name of and link to the calibration algorithm code (Interpolation, Polyval)
  4. names of and links to QC algorithm code associated with the data product
  5. link to QC algorithm LUT values
  6. if there are Human In the Loop QC variables in the data product, metadata explaining the Reasoning behind the HITL QC
  7. Instrument make, model
  8. Location at which the data deployment (lat, lon, depth)
In addition, if errors are detected in metadata values, the OOI Marine Operator or Project Scientist will be alerted and resolution will be tracked throught the trouble ticket system to update/correct metadata values.

3. The Data Manager searches for a data product which uses the latest calibration data to ensure new values are applied.

4. The UI displays the data product(s) with the associated metadata showing the latest calibration values have been applied.
