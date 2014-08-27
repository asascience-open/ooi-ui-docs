#![](http://www.rpsgroup.com/images/2012-specific/RPSlogo.aspx) OOI Web UI Construction 
# Infrastructure Asset Management

| Use Case ID | 001 |
| --- | --- |
| Name | Infrastructure Asset Management |
| Scope of Work | Asset Management UI |
| Actors | Science User |
| Requester |  |
| Description |  |

## Definition

## Assumptions

## Scenario

- Database that contains a comprehensive structure to describe and document the marine infrastructure:
  - Reference Designator
  - Array -> Platform -> Site -> Port -> Instrument

- Report Generator
  - SAF as a baseline
  - Report templates so that we can add more as necessary and desired
  - - Custom Reporting (SQL Query) - Do we want to simplify this for people? Not everyone knows SQL  Queries

- Forms for changing and editing table data
- Spreadsheet ingestion
- Potentially an ouch, but would be highly sought after because updating the metadata for 100+ instruments without some sort of bulk spreadsheet ingestion would cost hundreds of man-hours. Also having the Spreadsheet ingestion allows for  seamless asset addition to the database.