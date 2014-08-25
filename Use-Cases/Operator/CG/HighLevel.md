![Logo](http://asascience.com/images/logo.png)
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


# Marine Operator Turnover

| Use Case ID   |                                                           |
| ------------- | --------------------------------------------------------- |
| Name          | Marine Operator Turnover                                  |
| Description   | Tools to assist marine operators with watch turnover      |
| Actors        | CGSN Marine Operator                                      |

## Definition

Provide tools for the CGSN marine operators to maintain a watch log, and assist in watch turnover.

## Assumptions

## Scenario

Marine operators can keep a log of events that happened during the watch. The goal is the clear transfer of information between operators.

 - Who did what
 - What actions were taken
 - What actions are pending
 - Escalation of problems or notifications


