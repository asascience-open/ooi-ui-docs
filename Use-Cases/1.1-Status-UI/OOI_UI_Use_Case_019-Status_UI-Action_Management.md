#![](http://www.rpsgroup.com/images/2012-specific/RPSlogo.aspx) OOI Web UI Construction 
# Action Management

| Use Case ID | 019 |
| --- | --- |
| Name | Action Management                 |
| Scope of Work | Status UI |
| Actors | Marine Operator, Facility, OL |
| Requester | OL |
| Description | An action management system for tracking the resolutions of potential issues |

## 
Action management provides a method of tracking the problem resolution through assigned actions, engineering investigations, and FMEA.
 
## Assumptions
- Each individual user/actor will have their own Action Management Branch for reporting, delegating, and viewing actions needed.
- Redmine Based

## Scenario
1. An operator is logged in and an alarm pops up.
2. The operator acknowledged the issue and refers to previous training, experience, and/or issue mitigation procedures to decide on the appropraite action for resolution.
3. The operator opens action management and creates a new action.
4. The created action provides a step by step resolution procedure.
5. The operator assigns the action to a user, with a target date for completion, as well as users to be notified upon resolution.
6. Action management sends an SMS, email, or phonecall to let the assigned user know they have an outstanding action.
7. The assigned user logs in to the UI and goes to action management.
8. The user follows the step by step procedure for resolution.
9. Once resolved the assigned user closes the action. 
10. Action Management sends emails, sms, or phonecalls to notify the users who need to be notified that the problem has been resolved.


## Comments
- The system provides the user an interface for event, alert, and alarm resolution management.
- After an event, alert, or alarm that requires resolution occurs, the action management interface is populated with an action.
  - This action is assigned to a default user/actor based on the context of the event/alert/alarm. 
- The action management service disseminates the action delegation to the assigner and assignee.
- The user uses the interface to track the steps taken to resolution.
- Upon complete resolution, the user closes the action item and a message is disseminated to the appropriate stakeholder's notifying them of the compeltion.
