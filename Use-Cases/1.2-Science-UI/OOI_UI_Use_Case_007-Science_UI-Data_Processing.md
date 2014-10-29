#![](http://www.rpsgroup.com/images/2012-specific/RPSlogo.aspx) OOI Web UI Construction 
# Data Processing

| Use Case ID | 007 |
| --- | --- |
| Name | Data Processing |
| Scope of Work | Science UI |
| Actors | External Science User |
| Requester |  |
| Description | Some data must be processed before it is useful for the science user |

## Definition
Some data must be processed before it is useful for the science user.  

## Assumptions
Be able to retrieve, display and publish higher level data products (L1, L2) requiring complex data processing from OOI Infrastructure.

1. A scientist uses the UI to view and analyze higher order data.
2. OOI Infrastructure provides the processed data product when initiated by the user through the UI.

## Scenario 1 Scientist is interested in downloading some L2 data (salinity and density)
1. A science user logs into the UI and searches using a key word search for either sensor (CTD) or desired data product (salinity, density).
2. The science user selects the desired data which queries the OOI infrastructure database.
3. The displayed data product(s) may be visualized using the functions described in Use Case 003 (Graphing) or downloaded and saved to the user's local computer disk if desired.

Scenario 2 Science user is interested in downloading some L2 data derived from sensors, for a derived product. For this use case scenario, the science user wants to look at the ratio of chlorophyll fluorescence to the optical backscatter measured with EcoPuck mounted onboard OOI mooring. 
1. Science user logs into the UI and searches using a key word search for either sensor (EcoPuck) or for desired data product (chlorophyll fluorescence, optical backscatter).
2. The science user selects the desired data, which queries the OOI Infrastructure.
3. The displayed data product(s) may be visualized using the functions described in Use Case 003 (Graphing) or downloaded and saved tot he user's local computer disk if desired.


