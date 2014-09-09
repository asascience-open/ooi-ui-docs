#![](http://www.rpsgroup.com/images/2012-specific/RPSlogo.aspx) OOI Web UI Construction 
#Update Metadata in a Data Product

| Use Case ID | 032 |
| --- | --- |
| Name | Update Metadata in a Data Product |
| Scope of Work | Status UI |
| Actors: | The OOI cyberinfrastructure system; a Marine Operator or OOI Scientist |
| Requester | OL |
| Description: | Update values of all required metadata fields when a data product is updated  |


##Definition

OOI Data Products must have associated metadata which explains data provenance and which conforms to ocean science community standards. The metadata values must be up-to-date.

##Assumptions :

- The OOI Metadata Model has been created and baselined.
- The OOI Metadata Model includes metadata fields required by appropriate ocean science community standards.
- A metadata database has been created (e.g. PostgreS)
- The schema of the metadata database accommodates all metadata in the OOI Metadata Model

##Scenario

The following steps describe how the OOI cyberinfrastructure system will update the metadata.

Steps:

1. When a data product is reprocessed, update all data product metadata values which have changed.
2. Data product metadata shall include:


  1. Name of and link to the Data Product Specification document
  2. name of and link to the Data Product Algorithm code
  3. Name of and link to the calibration algorithm code (Interpolation, Polyval)
  4. names of and links to QC algorithm code associated with the data product
  5. link to QC algorithm LUT values
  6. if there are Human In the Loop QC variables in the data product, metadata explaining the Reasoning behind the HITL QC
  7. Instrument make, model
  8. Location at which the data were collected (lat, lon, depth)

In addition, if errors are detected in metadata values, an OOI Marine Operator or Project Scientist may need to update/correct metadata values via a user interface.
