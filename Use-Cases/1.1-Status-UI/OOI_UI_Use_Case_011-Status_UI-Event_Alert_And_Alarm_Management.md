#![](http://www.rpsgroup.com/images/2012-specific/RPSlogo.aspx) OOI Web UI Construction 
# Event, Alert, and Alarm Management

| Use Case ID | 011 |
| --- | --- |
| Name | Event, Alert, and Alarm Management                 |
| Scope of Work | Status UI |
| Actors | RSN Marine Operator, CG Marine Operator, EA Marine Operator, Science User |
| Requester | OL |
| Description | Allows user to obtain specific automated responses to data thresholds or engineering data limits |

## Definition
The actor may configure alerts and alarms to to be brought to the user's attention based off of an occurring event.  An alert denotes an event that requires attention.  An alarm denotes an event that requires an immediate action and the system may take steps to notify key personnel.  Action management provides a method of tracking the event/alert/alarm resolution.  See [OOI UI Use Case 019 - Action Management](OOI_UI_Use_Case_019-Status_UI-Action_Management.md) for more on Action Management

## Assumptions
- Observatory Management System (OMS) monitors and publishes many events related to monitoring of the marine assets.
- Every actor and asset type will have different requirements for events that trigger an alert or alarm.

## Scenario
- The system captures OMS events and integrates them with event, alert, and alarm management.
- The user will be provided with a way to customize events/alert/alarm criteria
- The customization of events/alert/alarm criteria for each asset is based on the following event tiers: 
- The system allows the user/actor to customize the dissemination of events/alerts/alarms for each criteria
- The dissemination methods include:
  - Emails
  - SMS Messaging
  - Visual Indications
  - Log Files
- After the user/actor defines the event/alert/alarm criteria for an asset Event, Alert, and Alarm Management will search for occurring events, filter them, and trigger alerts/alarms based off the defined criteria.
- The system will disseminate the events, alerts, and alarms to the actors/users based on the defined dissemination criteria.
- A user will also be provided the ability to subscribe/unsubscribe to an existing alert/alarm.

#### Example of tiered categories

- Tier 1 
  - Geolocation 
  - Telemetry
  - Communications
- Tier 2
  - Power System Controller
  - Status of Platform Controllers
  - CPM, DCL, STC, and MPEA status
  - MMP Profiling Function
- Tier 3
  - Instrument Function
  - MMP profiling function

##Comments

- This use case must take place within the User Interface of OOI Net
- Users must not get flooded with alerts - implementation is key
- User definition of criteria is not possible at this time
