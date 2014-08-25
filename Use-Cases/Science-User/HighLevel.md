# Graphing

| Use Case ID   |                                                           |
| ------------- | --------------------------------------------------------- |
| Name          | Graphing                                                  |
| Description   |                                                           |
| Actors        | Science User                                              |

## Definition

## Assumptions

## Scenario

- Multiple variable graphing
- Plot stacking from multiple instruments and variables
- 3D Plots to include extra dimensions like Depth and Profile Views
- See Rutgers PPT for examples

# Data Provisions

| Use Case ID   |                                                           |
| ------------- | --------------------------------------------------------- |
| Name          | Data Provisions                                           |
| Description   |                                                           |
| Actors        | Science User                                              |

## Definition

## Assumptions

## Scenario

- Get the data to the users
- Preferably a common interface like OPeNDAP via ERDDAP AND Thredds
 - ERDDAP has a limited data model that may not fit all the data we have to
   offer
 - We could even use a custom OPeNDAP service to serve netcdf files
 - Or we could just use thredds

# ERDDAP

| Use Case ID   |                                                           |
| ------------- | --------------------------------------------------------- |
| Name          | ERDDAP                                                    |
| Description   |                                                           |
| Actors        | Science User                                              |

## Definition

## Assumptions

## Scenario

- ERDDAP is a community standard and has already been a known interface for R2
  and R3, and we shouldn't break a known interface

# Map Overlays

| Use Case ID   |                                                           |
| ------------- | --------------------------------------------------------- |
| Name          | Map Overlays                                              |
| Description   |                                                           |
| Actors        | Science User                                              |

## Definition

## Assumptions

## Scenario

- The standard map used in the interface should be able ot include overlays
- I would suggest even letting users add their own layers through WMS endpoints
  or even tile servers (stretch maybe)

# Data Processing

| Use Case ID   |                                                           |
| ------------- | --------------------------------------------------------- |
| Name          | Data Processing                                           |
| Description   |                                                           |
| Actors        | Science User                                              |

## Definition

## Assumptions

## Scenario

- Be able to retrieve, display and publish higher level data products requiring
  complex data processing from uFrame.
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

