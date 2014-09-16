#![](http://www.rpsgroup.com/images/2012-specific/RPSlogo.aspx) OOI Web UI Construction 
# Monitor system health and status

| Use Case ID | 020 |
| --- | --- |
| Name | Monitor system health and status                |
| Scope of Work | Status UI |
| Actors | Marine Operator, Science User, Facility, OL|
| Requester | OL |
| Description | An "assets at a glance" landing page for marine operators |

## Definition
An "assets at a glance" landing page for marine operators to view all assets currently deployed in the OOI.
 
## Assumptions
- Both hardware and software status messages are generated and transmitted by the system's various components.
- There is a consolidated status message vocabulary and assignments used throughout the program.
- The dictionary of status entries is suitable for sorting and selective display as a function of, at a minimum: item, location, status, level of issue, multiple states
- This function is also related to and interacts with the alert/alarm functions

## Scenario
- When an operator uses the status UI they are provided with a dhasboard view of OOI assets.
  - This view will show:
    - Name
    - Status
    - Power usage/ power availability
  - On this view the operator is able to:
    - Toggle on/off display of assets
    - Sort by paramters
    - Mouse over to display basic information
      - Lat/Lon
      - Deploy Date
- Time data of these statuses are provided to the user as well.



- As an alternative view, the operator is provided a world map that displays all of the currently deployed assets.
- The world map supports overlays that are selectable by the operator.
- On this world map, the operator can:
  - Zoom and Pan
    - Zooming changes the level of detail displayed (arrays, platform, nodes, components)
  - Toggle on/off display of assets
  - Mouse over the asset to display basic information.
    - Status
    - Deploy Date
    - Name
    - Power usage/ power availability
  - Drill down from higher level assets (e.g. arrays) to lower level assets (e.g. components)

1. A critical server at the shore station abruptly powered off and a new, backup, server assumed responsibility - data may or may not have stopped flowing. This is an urgent event that requires immediate investigation and may affect capture of science data.

Steps

1. Both the RSN MO and the CI O&M technician receive an alert of this HW change.
2. They both utilize "pings" in an attempt to contact the server; but fail to get a response.
3. The RSN MO checks other telemetry instruments at the shore station (fire, water, temperature, cameras) to identify if there are other suspicious issues; the event seems isolated.
4. The MO and CI technician confer over email and decide to try a reboot; the reboot fails without response.
5. At this point, and per procedure, the MO opens a TR and contacts the RSN O&M Lead to explain the situation. 
6. The next day a person investigates, fixes the fault and eventually closes the TR.

2. A buoy has exceeded its watch circle which suggests it has broken free from its mooing. This is an emergent situation that poses a hazard to navigation

Steps

1. The MO receives an alarm for the above event. 
2. The MO quickly reviews the telemetry to determine if it could be a false alarm but finds no evidence of a false alarm.
3. The MO begins the applicable procedure and begins execution by first notifying the MIO O&M Lead and opening a TR.
4. The MO confers with the CI O&M technician (if available) to double check the telemetry and investigate alternative possibilities.
5. The MIO O&M Lead assumes responsibility and executes the "Loose at sea, Asset Procedure." If the MIO O&M Lead is not immediately available, the procedure identifies the second and third person to assume responsibility and subsequent actions.

3. During a dive, a glider detects water in the electronics bay, auto-aborts the dive, surfaces in a shipping lane and sends a distress signal via satellite. This is a safety event and an emergent situation requiring immediate action.

Steps

1. The MO receives an alarm for the above event. 
2. The MO quickly reviews the telemetry to determine if it could be a false alarm but finds no evidence of a false alarm.
3. The MO begins executing the applicable procedure for a surfaced glider and first notifies the MIO O&M Lead and opening a TR.
4. The MO confers with the CI O&M technician (if available) to double check the telemetry and investigate possibilities. The glider location is determined from telemetry and it is identified to be a hazard to shipping.
5. The MIO O&M Lead assumes responsibility and executes the "Loose at sea, Hazard to Shipping, Asset Procedure." This would include changing the life-cycle state of the platform. If the MIO O&M Lead is not immediately available, the MO executes the procedure.

4. An instrument detects an underwater event of scientific interest, communicates to shore and receives instructions to change sampling intervals and/or movement to investigate. Intensive monitoring is required to avoid consuming irreplaceable power or other resources.

Steps

1. Either scientists (internal or external) or the O&M MO detects a major and unusual event. The Observatory Director, MIO O&M Director, MIO O&M Leads and OOI scientists (those available and based on the time scale of the event and need for response) quickly confer and jointly decide the value and initial impacts (both science and O&M costs) of changing various instrument sampling rates and relocating mobile assets to gather unusual data. A lead scientist and MIO MO are assigned to quickly develop a proposed new mission that includes assets involved, activities of each and end of mission date/time. 
2. The proposed new mission is evaluated by affected groups- the MIO and CI for impact. Available additional scientists or SMEs are requested to provide a quick review. The conclusion is that the recommended mission plan (with modest changes) should proceed.
3. The revised mission plan is presented to NSF for approval and approved- unless this event and change is already included in an established procedure.
4. The MIO O&M Director transmits approval to the MIO O&M Lead who then directs the MO to execute the new mission plan. 
5. The MIO OD also informs the webmaster of the event and the MIO OD, with the MIO O&M Lead and OOI scientists develop and post an announcement on the OOI website.
6. The new mission plan involves changing the sampling rates on six instruments and moving three gliders to a different location. The MOs implement these changes per established procedures.
7. The MOs then closely monitor the reassigned assets for both data performance and operational consequences of these new assignments.
8. At the end of the mission, the assets are returned to their previously defined sampling rates or to those rates as specified in the amended mission plan. The webmaster post and announcement of the changed configurations.

5. A recent deployment included an externally funded and new PI instrument. It is unknown exactly how the rest of the mooring will respond. Close monitoring is required for both the mooring and the affected data path to ensure the new instrument and data do not affect the rest of the system.

Steps

1. Following deployment of the mooring, the MIO MO and the CI O&M technician execute the "Special PI Attached Mooring Monitoring Procedure." The MIO MO focuses on the mooring health, safety and operation while the CI technician focuses on the data path and CI system functions. (New PI duties TBD)
2. Depending on the length of the PI activity and assessed possible impact to the mooring, initial close monitoring may proceed from hourly to daily to weekly if all operations appear nominal.
3. The MIO and CI technicians have pre-approved contingency actions that they can take to safeguard the deployed assets and the data path of OOI products.

6. There is a need to set/change alerts/alarms and then monitor them closely to make sure the changes were correct and that the item of interest is being properly auto-monitored and reported by the system. This scenario applies to

- All sea assets
- All land assets
- All science products
- All operational leased assets- e.g., comms

Steps

1. The MIO MO, per direction of the MIO O&M Lead, enters all initial alarms settings (thresholds) for MIO assets.
2. The MIO O&M Lead establishes and enters automated responses and/or response procedures for MIO assets.
3. The CI technician, per direction of the CI O&M Lead, enters all initial alarms settings (thresholds) for CI assets and communications lines.
4. The CI O&M Lead establishes and enters automated responses and/or response procedures for CI assets and communications lines.
5. The OOI scientists establish and enter all initial alarms settings (thresholds) for all science data/data product values and QC results.
6. The O&M Leads (CI and all MIOs) and OOI scientists create all alarm notifications for their teams.
7. The O&M Leads (CI and all MIOs) and OOI scientists monitor subscriptions .
8. The O&M Leads (CI and all MIOs) and OOI scientists respond per procedures. These responses include examination of data streams, examination of telemetry, trouble shooting, all steps of data path from instrument to data delivery, generate/provide reports, generate and report performance metrics and issues, search, filter and download data, view/edit metadata, update of procedures, and updating of alert settings.

