#![](http://www.rpsgroup.com/images/2012-specific/RPSlogo.aspx) OOI Web UI Construction 
#Respond to Trouble Ticket

| Use Case ID | 031 |
| --- | --- |
| Name | Respond to Trouble Ticket |
| Scope of Work | Status UI |
| Actors: | Facility |
| Requester | OL |
| Description: | Provides an interface for the viewing of and response to a Trouble Ticket  |


##Definition

There needs to be a system for the viewing of and response to trouble tickets filed by users.

##Assumptions

- A supported browser is used
- Red Mine is used

##Scenario

The following steps describe one way the actor would utilize the system to accomplish this task.

Steps:

1. User has already filed a Trouble Ticket
2. Trouble Ticket is registered by the Trouble Ticket Service and then delegated to an appropriate person for resolution
3. The person delegated the Trouble Ticket fixes the issue
4. Once fixed, the fixer registers the fix in the Trouble Ticket Service and closes the ticket
5. The Trouble Ticket service logs the completion and alerts the original user of the fix
6. Any user with access to the trouble ticket system is able to search for and retrieve open or closed tickets
