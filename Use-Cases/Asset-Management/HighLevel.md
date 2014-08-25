# Infrastructure Asset Management

| Use Case ID   |                                                           |
| ------------- | --------------------------------------------------------- |
| Name          | Infrastructure Asset Management                           |
| Description   |                                                           |
| Actors        | Science User                                              |

## Definition

## Assumptions

## Scenario

- Database that contains a comprehensive structure to describe and document the marine infrastructure:
 - Reference Designator
 - Array -> Platform -> Site -> Port -> Instrument
- Report Generator
 - SAF as a baseline
 - Report templates so that we can add more as necessary and desired
 - Custom Reporting (SQL Query) - Do we want to simplify this for people? Not everyone knows SQL    Queries
- Forms for changing and editing table data
- Spreadsheet ingestion
 - Potentially an ouch, but would be highly sought after because updating the
   metadata for 100+ instruments without some sort of bulk spreadsheet
   ingestion would cost hundereds of man-hours.  ALso having the Speadsheet ingestion allows for    seamless asset addition to the database.

# Deployment Planning and Management

| Use Case ID   |                                                           |
| ------------- | --------------------------------------------------------- |
| Name          | Deployment Planning and Management                        |
| Description   |                                                           |
| Actors        | Science User                                              |

## Definition

## Assumptions

## Scenario

- Able to identify physically where the instrument is, has been and is planned to be
- Maybe a map?
- Think, given a serial number, or serial numbers, provide planning capabilities
- Asset State:
 - Planned
 - Deployed
 - Status OK
 - Status BAD
 - Recovered
 - Testing
 - Vendor
 - Bench
- Tie this information into other displays
 - When looking at the port configuration also be able to come see this
   instruments specific information


