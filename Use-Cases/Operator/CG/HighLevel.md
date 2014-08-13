# Fixed Platform Status Operations for Uncabled Surface Moorings

| Use Case ID |     |
|-------------|---------------------------------------------------------|
| Name | Fixed Platform Status Operations for Uncabled Surface Moorings |
| Description |                                                         |
| Actors | CGSN Marine Operator                                         |

## Definition

## Assumptions

## Scenario

Marine Operator can identify the health and status of the platform. The items of interest that compose an overall status
of the platform can be broken into three tiers. Tier 1 items are the most important factors for observing the health of
the platform. A failure observed in a tier 1 item would be indicative of serious platform health issues.

__Examples for Tier 1 items__:

 - Geolocation, the platform remains within the geofence.
 - Telemetry and Communication Status
   - Fleed Broadband
   - Iridium ISU
   - Iridium SBD
   - Beacons
   - Instruments to the CPM or STC
   - DCL link and Schedule Variance

__Example for Tier 2 items__:

 - Power System Controller
   - Battery Charge, Charge Cycle
   - Voltage and Current Draws
 - Status of platform controllers
 - CPM, DCL, STC, MPEA status
   - Voltag, humidity, leak-detect, port status
   - Error codes
   - Anomalies and trends
 - MMP Profiling Function

__Example for Tier 3 items__:

 - Instrument Function
  - Data file presence, size
  - Data range and trend
  - Anomalies and trends
  - Specific instrument outputs
 - MMP profiling function



