#![](http://www.rpsgroup.com/images/2012-specific/RPSlogo.aspx) OOI Web UI Construction 
# Data Processing

| Use Case ID | 007 |
| --- | --- |
| Name | Data Processing |
| Scope of Work | Science UI |
| Actors | Science User |
| Requester |  |
| Description | Some data must be processed before it is useful for the science user |

## Definition
Some data must be processed before it is useful for the science user.  One example is conductivity data from a CTD being processed to salinity.

## Assumptions
Be able to retrieve, display and publish higher level data products (L2) requiring complex data processing from uFrame.

1. A scientist uses the UI to view and analyze higher order data.
2. uFrame provides the processed data product when initiated by the user through the UI.

## Scenario
Example with colocated instruments that combine to make L2 parameters
1. A science user logs into the UI and searches for OPTABSN and OPTATTN data product.
2. The science user selects the desired data which queries the uFrame database and applies the appropriate algorithm
3. The OPTABSN and OPTATTN data product is displayed with the higher level data products from colocated instruments.
4. If the data from one of the instruments is unavailable or invalid, an error message is displayed with description of the exception for trouble ticket reporting.
5. The science user examines the data products with the corresponding metadata (ie algorithm version, valid dates, author, instrument POC)
6. The science user may add notes or comments to the data product or request more information via trouble ticket system.
7. The displayed data product(s) may be downloaded and saved to the user's local computer disk if desired. 

Example with Temporally Aware Data Processing
1. A science user logs into the UI and searches for the METBK data product.
2. The science user selects the desired data which queries the uFrame database and applies the appropriate QA algorithm
3. The METBK data product is displayed with the QA algorithm applied.
4. If the data from the METBK instrument is unavailable or invalid, an error message is displayed with description of the exception for trouble ticket reporting.
5. The science user examines the data product with the corresponding metadata (ie algorithm version, valid dates, author, instrument POC)
6. The science user may add notes or comments to the data product or request more information via trouble ticket system.
7. The displayed data product(s) may be downloaded and saved to the user's local computer disk if desired. 

Example with Platform Integrated Parameters
1. A science user logs into the UI and searches for a Platform data product (ie Gliders that provide lat/lon to attached sensors, Wire Following Profilers that provide parameters for ADCP instrument).
2. The science user selects the desired data which queries the uFrame database and applies the appropriate algorithm with parameters provided by the Platform
3. The data product is displayed with the algorithm applied.
4. If the required data parameters from the platform is unavailable or invalid, an error message is displayed with description of the exception for trouble ticket reporting.
5. The science user examines the data product with the corresponding metadata (ie algorithm version, valid dates, author, instrument POC)
6. The science user may add notes or comments to the data product or request more information via trouble ticket system.
7. The displayed data product(s) may be downloaded and saved to the user's local computer disk if desired. 


