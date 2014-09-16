#![](http://www.rpsgroup.com/images/2012-specific/RPSlogo.aspx) OOI Web UI Construction 
# Event, Alert, and Alarm Management

| Use Case ID | 011 |
| --- | --- |
| Name | Event, Alert, and Alarm Management                 |
| Scope of Work | Status UI |
| Actors | Marine Operator, Facility, OL |
| Requester | OL |
| Description | Allows user to obtain specific automated responses to data thresholds or engineering data limits |

## Definition
The actor may configure alerts and alarms to to be brought to the user's attention based off of an occurring event.  An alert denotes an event that requires attention.  An alarm denotes an event that requires 24/7 action.  Action management provides a method of tracking the event/alert/alarm resolution.  See [OOI UI Use Case 019 - Action Management](OOI_UI_Use_Case_019-Status_UI-Action_Management.md) for more on Action Management

## Assumptions
- Observatory Management System (OMS) monitors and publishes many events related to monitoring of the marine assets.
- Every actor and asset type will have different requirements for events that trigger an alert or alarm.

## Scenario
Scenario 1 - Operator:
1. Operator logs in to the UI
2. Operator goes to the event, alert, and alarm management service.
3. Operator creates a custom alert to warn the operator if a specific asset leaves a provided bounding box.
4. Operator creates a custom alarm to  warn the operator if a specific asset leaves a provided bounding box.
5. Some time later the asset drifts outside the alert bounding box parameters.
6. The UI provides a visual/audio cue to let the operator know that the asset has moved outside the bounding box.
7. The Operator acknowledges the alert and returns to work without creating an action for resolving the alert.
8. The asset continues to drift and leaves the alarm bounding box.  
9. The UI provides a visual/audio cue to let the operator know that the asset has has moved outside the alarm bounding box.  
10.  Depending on the customized alarm, emails, SMS, or phonecalls may also be made to notify people of the alarm.  
11. The Operator is not able to return to work without both acknowledging the alarm, as well as creating an action in action management to mitigate the issue.

Scenario 2 - Facility:
1. A facility user logs in to the UI
2. The facility user creates an alarm to notify themself and all active operators when an asset's voltage reaches a certain level.
3. The facility user creates an alert to notify themself and specific OL accounts when an asset has been deployed for over 100 days.
4. The asset's voltage drops below the threshold, but the facility user is not logged in.
5. The UI sends sms, email, or phonecalls to warn the facility user.
6. The UI provides a  visual/audio cue to let the operator know that the asset's voltage ahs dropped below the threshold.  
7.  Depending on the customized alarm, emails, SMS, or phonecalls may also be made to notify people of the alarm.  
8. The Operator is not able to return to work without both acknowledging the alarm, as well as creating an action in action management to mitigate the issue.
9. Some time later another asset hits the 100 day milestone.  The facility user and OL account is emailed with a prewritten message informing of the 100 day milestone.

Scenario 3 - OL:
1. An OL user logs in to the UI
2. The OL user creates an alert to be notified whenever an asset is deployed.
3. The OL user creates an alert to be notified whenever an asset is removed from service.
4. The OL user recieves an SMS each time the alert occurs.


## Comments
- The system captures OMS events and integrates them with event, alert, and alarm management.
- The user will be provided with a way to customize events/alert/alarm criteria
- The customization of events/alert/alarm criteria for each asset is based on the following event tiers: 
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
- The system allows the user/actor to customize the dissemination of events/alerts/alarms for each criteria
- The dissemination methods include:
  - Emails
  - SMS Messaging
  - Visual Indications
  - Log Files
- After the user/actor defines the event/alert/alarm criteria for an asset Event, Alert, and Alarm Management will search for occurring events, filter them, and trigger alerts/alarms based off the defined criteria.
- The system will disseminate the events, alerts, and alarms to the actors/users based on the defined dissemination criteria.
- A user will also be provided the ability to subscribe/unsubscribe to an existing alert/alarm.
- This use case must take place within the User Interface of OOI Net
- Users must not get flooded with alerts - implementation is key
- User definition of criteria is not possible at this time
