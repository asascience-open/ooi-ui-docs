# RSN Command and Control

| Use Case ID   |                                                           |
| ------------- | --------------------------------------------------------- |
| Name          | RSN Command and Control                                   |
| Description   |                                                           |
| Actors        | RSN Marine Operator                                       |

## Definition

## Assumptions

## Scenario

- Status screens:
 - Port status and power information
   - Temperature
   - Current
   - Voltage
 - Issue commands to the platforms
 - Port power control
 - Over-current limits
 - Platform state managemnt (doesn't really follow a FSM)
 - Mission Executive
 - Event monitoring and status parameters
  - Status parameters come from the OMS
- Bridge the gap between the platform control and instrument management 
 - Immediately transition to instrument control from a platform/port page
- Port Schedules
- Events
- Network View, so something like the wire-diagram that shows how the network
  is physically laid out.

# Event, Alert, Alarm Management

| Use Case ID   |                                                           |
| ------------- | --------------------------------------------------------- |
| Name          | Event and Alert Management                                |
| Description   |                                                           |
| Actors        | RSN Marine Operator                                       |

## Definition

## Assumptions

## Scenario

- Observatory Management System (OMS) monitors and publishes many events
  related to monitoring of the marine assets. We need to be able to capture
  those events and integrate with event management.
- Searching for events
- Filtering events
- Evenet dissemination
 - How will we get the events to the operators?


# Management Planning and Asset Management

| Use Case ID   |                                                           |
| ------------- | --------------------------------------------------------- |
| Name          | Management Planning and Asset Management                  |
| Description   |                                                           |
| Actors        | RSN Marine Operator                                       |

## Definition

## Assumptions

## Scenario

- A planning tool integrated with asset management
 - Plan for deployments
 - Observe current location for marine assets and their current state
 - Contact Bob for use of his language in this regard
- Marine Asset State
 - Planning
 - Deployed
 - Status OK
 - Status Bad
 - Recovered
 - Testing
 - Bench


# External Interfaces

| Use Case ID   |                                                           |
| ------------- | --------------------------------------------------------- |
| Name          | External Interfaces                                       |
| Description   |                                                           |
| Actors        | RSN Marine Operator                                       |

## Definition

## Assumptions

## Scenario

- Seismic data being shared with Iris and UI providing links and some degree of
  integration with IRIS.



# Mission Executive

| Use Case ID   |                                                           |
| ------------- | --------------------------------------------------------- |
| Name          | Mission Executive                                         |
| Description   |                                                           |
| Actors        | RSN Marine Operator                                       |

## Definition

## Assumptions

## Scenario

- Mission Executive Capabilities
- Create, Define, Review and Schedule Missions to be executed by platforms

# User Annotations and User Log

| Use Case ID   |                                                           |
| ------------- | --------------------------------------------------------- |
| Name          | User Annotations and User Log                             |
| Description   |                                                           |
| Actors        | RSN Marine Operator                                       |

## Definition

## Assumptions

## Scenario

- Be able to write a watch log of the events that transpired during the watch
- Be able to ann

# 3D Scene Management for Marine Assets

| Use Case ID   |                                                           |
| ------------- | --------------------------------------------------------- |
| Name          | 3D Scene Management for Marine Assets                     |
| Description   |                                                           |
| Actors        | RSN Marine Operator                                       |

## Definition

## Assumptions

## Scenario

- Display a 3D scene for the marine assets to assist operators in visualizing
  and quickly identifying faults in the infrastructure.


# HD Video Camera Feed

| Use Case ID   |                                                           |
| ------------- | --------------------------------------------------------- |
| Name          | HD Video Camera Feed                                      |
| Description   |                                                           |
| Actors        | RSN Marine Operator                                       |

## Definition

## Assumptions

## Scenario

- Provide HD Video Feed to both Science Users and Marine Operators

# QA/QC Data Evaluation

| Use Case ID   |                                                           |
| ------------- | --------------------------------------------------------- |
| Name          | QA/QC Data Evaluator                                      |
| Description   |                                                           |
| Actors        | Data Integrator                                           |

## Definition

## Assumptions

## Scenario


