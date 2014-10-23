#![](http://www.rpsgroup.com/images/2012-specific/RPSlogo.aspx) OOI Web UI Construction 
#Add ancillary data from OOI cruises

| Use Case ID | 023 |
| --- | --- |
| Name | Add ancillary data from OOI cruises |
| Scope of Work | Science UI |
| Actors | Operator, Science, Data Manager  |
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

1. Operator places the results in a pre-formatted OOI cruise spreadsheet, with a link to the sample collection and analysis protocols used.
2. Operator logs into the UI and searches for and nagivates to array/platform(s) the cruise apples to on the Science UI screen.
3. Operator selects option to upload ancillary data. OOI cruise spreadsheet is added to the data model. The link to this spreadsheet is created in the metadata for all related data products.
4. If an error occurs in the databse injection (wrong data type, field too long, etc.) the operator is informed of the failure along with verbage to explain the error. 

