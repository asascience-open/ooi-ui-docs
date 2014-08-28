#![](http://www.rpsgroup.com/images/2012-specific/RPSlogo.aspx) OOI Web UI Construction 
# Action Management

| Use Case ID | 019 |
| --- | --- |
| Name | Action Management                 |
| Scope of Work | Status UI |
| Actors | RSN Marine Operator, CG Marine Operator, EA Marine Operator, Science User |
| Requester | OL |
| Description | An action management system for tracking the resolutions of potential issues |

## Definition
Action management provides a method of tracking the problem resolution through assigned actions, engineering investigations, and FMEA.
 
## Assumptions
- Each individual user/actor will have their own Action Management Branch for reporting, delegating, and viewing actions needed.
- JIRA Based

## Scenario
- The system provides the user an interface for event, alert, and alarm resolution management.
- After an event, alert, or alarm that requires resolution occurs, the action management interface is populated with an action.
  - This action is assigned to a default user/actor based on the context of the event/alert/alarm. 
- The action management service disseminates the action delegation to the assigner and assignee.
- The user uses the interface to track the steps taken to resolution.
- Upon complete resolution, the user closes the action item and a message is disseminated to the appropriate stakeholder's notifying them of the compeltion.
