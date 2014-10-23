#![](http://www.rpsgroup.com/images/2012-specific/RPSlogo.aspx) OOI Web UI Construction 
#Update Metadata in a Data Product

| Use Case ID | 032 |
| --- | --- |
| Name | Update Metadata in a Data Product |
| Scope of Work | Status UI |
| Actors: | Marine Operator, Science |
| Requester | OL |
| Description: | Update values of all required metadata fields when a data product is updated  |


##Definition

OOI Data Products must have associated metadata which explains data provenance and which conforms to ocean science community standards. The metadata values must be up-to-date.

##Assumptions :

- The OOI Metadata Model has been created and baselined.
- The OOI Metadata Model includes metadata fields required by appropriate ocean science community standards.
- A metadata database has been created 
- The schema of the metadata database accommodates all metadata in the OOI Metadata Model

##Scenario

The following steps describe how the operator or project scientist will update the metadata.


1. A Data Product Algorithm has been updated with new calibration data. 
   a. The Data Manager logs into the UI
   b. The Data Manager searches for and navigates to the platform the new calibration data should be applied
   c. The Data Manager views current calibration data and enters new calibration values
   d. The UI prompts the user for required metadata values (ie valid dates, DPA code or ID, location)
   e. The uFrame database stores the new calibration values
2. When the new calibration is applied to the OOINet system, the uFrame database will update all data product metadata values which have changed. Data product metadata shall include:
  1. Name of and link to the Data Product Specification document
  2. name of and link to the Data Product Algorithm code
  3. Name of and link to the calibration algorithm code (Interpolation, Polyval)
  4. names of and links to QC algorithm code associated with the data product
  5. link to QC algorithm LUT values
  6. if there are Human In the Loop QC variables in the data product, metadata explaining the Reasoning behind the HITL QC
  7. Instrument make, model
  8. Location at which the data were collected (lat, lon, depth)
In addition, if errors are detected in metadata values, the OOI Marine Operator or Project Scientist will be alerted and resolution will be tracked throught the trouble ticket system to update/correct metadata values.
3. The Data Manager searches for a data product which uses the latest calibration data to ensure new values are applied.
4. The UI displays the data product(s) with the associated metadata showing the latest calibration values have been applied.
