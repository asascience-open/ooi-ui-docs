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

## Scenario
Be able to retrieve, display and publish higher level data products requiring complex data processing from uFrame.

1. A scientist uses the UI to observe higher order data.
2. The UI is provided the higher order data from uFrame, already processed.

The following data might be desired by a scientist:
- Complex Data Processing Includes:
  - Colocated Instruments that combine to make L2 parameters
    - OPTABSN
    - OPTATTN

  - Temporally Aware Data Processing
    - QA Algorithms
    - METBK

  - Platform Integrated Parameters
    - Gliders (Lat/Lon)
    - Wire Following Profilers
      - ADCPs need direction from the WFP to create the bins

