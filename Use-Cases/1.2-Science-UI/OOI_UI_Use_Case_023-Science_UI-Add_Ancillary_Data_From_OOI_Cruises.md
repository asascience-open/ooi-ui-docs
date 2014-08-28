#![](http://www.rpsgroup.com/images/2012-specific/RPSlogo.aspx) OOI Web UI Construction 
#Add ancillary data from OOI cruises

| Use Case ID | 023 |
| --- | --- |
| Name | Add ancillary data from OOI cruises |
| Scope of Work | Science UI |
| Actors | Internal science user (MIO-SU), MIO O&M Lead, marine operator (MIO-MO), OOI webmaster (CI-WM).  |
| Requester | OL |
| Description |  |

##Definition
Ancillary data includes all information outside the DATA PATH of OOI Net. Examples include

- Cruise plan
- Cruise report (links to at-sea sampling results, ROV reports, and underway ship data in the R2R system)
- As-built TDP (e.g., Array physical configuration)
- Instrument tables (what, where, products, sample rates)
- Instrument and data product metadata tables 
- Spreadsheets and community supported formats with analytical results from sample analysis (chl, oxygen, etc)
- Data files from all CTD casts
- Deployment/recovery images and video

##Assumptions

- Directory/file structure/document control system is in place for upload and storage of ancillary data/documents.
- User Interface provides transparent linkage between OOI Net data pages and the OOI Net ancillary data/doc pages 

##Scenario
User needs to ADD information to the ancillary data collection from Pioneer II deployment/recovery cruise (April 2014).

User completes processing 162 water samples for Chlorophyll _a_ analysis from the nine CTD casts conducted during the cruise (triplicate samples at each of the six depths sampled per cast) in support of calibration procedures. 

Actions to ADD these ancillary data to the OOI permanent record:

1. MIO-SU places the results in a pre-formatted OOI cruise spreadsheet, with a link to the sample collection and analysis protocols used.
2. MIO O&M Lead (or designee) cross-checks spreadsheet for accuracy (quality), signs off, creates action item (TR?) and sends/assigns to webmaster.
3. OOI webmaster sees opened action item/TR, and per procedure uploads to the OOI website under Configuration Management control. 
4. MIO O&M Lead validates (signs off) that the file has been uploaded to the correct location within the directory structure and confirms that the file can be retrieved without error. Then closes action item/TR
in the User Interface of OOI, in this case the data documentation branch of the OOI website