# Event, Alert, and Alarm Management

| Use Case ID | 011 |
| --- | --- |
| Name | Event, Alert, and Alarm Management                 |
| Scope of Work | Status UI |
| Actors | RSN Marine Operator, CG Marine Operator, EA Marine Operator |
| Requester | OL |
| Description | An event, alert, and alarm system for informing users of potential issues |

# Definition
The actor may configure alerts and alarms to to be brought to the user's attention based off of an occurring event.  An alert donates an event that requires attention.  An alarm denotes an event that requires 24/7 action.  Action management provides a method of tracking the event/alert/alarm resolution.  See [OOI UI Use Case 019 - Action Management](OOI_UI_Use_Case_019-Status_UI-Action_Management.md) for more on Action Management

# Assumptions
- Every actor and asset type will have different requirements for events that trigger an alert or alarm.

# Scenario
Observatory Management System (OMS) monitors and publishes many events related to monitoring of the marine assets. There is a need to be able to capture those events and integrate with event management.  Event, Alert, and Alarm Management will need to be able to search for occurring events, filter them, and trigger alerts/alarms based off of user/actor defined event criteria.  This criteria needs to be customizeable based on the following tiers: 
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

Also, the event/alert/alarm dissemination needs to be customizeable.  The dissemination methods should include:
- Emails
- SMS Messaging
- Visual Indications
- Log Files
