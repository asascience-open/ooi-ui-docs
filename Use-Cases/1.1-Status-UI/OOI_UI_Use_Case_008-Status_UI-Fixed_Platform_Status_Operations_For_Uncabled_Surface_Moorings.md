#![](http://www.rpsgroup.com/images/2012-specific/RPSlogo.aspx) OOI Web UI Construction 
# Fixed Platform Status Operations for Uncabled Surface Moorings

| Use Case ID | 008 |
| --- | --- |
| Name | Fixed Platform Status Operations for Uncabled Surface Moorings |
| Scope of Work | Status UI |
| Actors | CGSN Marine Operator |
| Requester | CG |
| Description | Display the health and status of the Uncabled Surface Moorings|

## Definition

## Assumptions

## Scenario

Marine Operator can identify the health and status of the platform. The items of interest that compose an overall status of the platform can be broken into three tiers. Tier 1 items are the most important factors for observing the health of the platform. A failure observed in a tier 1 item would be indicative of serious platform health issues.

### Examples for Tier 1 items

- Geolocation, the platform remains within the geofence.
- Telemetry and Communication Status
  - Fleed Broadband
  - Iridium ISU
  - Iridium SBD
  - Beacons
  - Instruments to the CPM or STC
  - DCL link and Schedule Variance

### Example for Tier 2 items

- Power System Controller
  - Battery Charge, Charge Cycle
  - Voltage and Current Draws

- Status of platform controllers
- CPM, DCL, STC, MPEA status
  - Voltage, humidity, leak-detect, port status
  - Error codes
  - Anomalies and trends

- MMP Profiling Function

### Example for Tier 3 items

- Instrument Function
  - Data file presence, size
  - Data range and trend
  - Anomalies and trends
  - Specific instrument outputs

- MMP profiling function
