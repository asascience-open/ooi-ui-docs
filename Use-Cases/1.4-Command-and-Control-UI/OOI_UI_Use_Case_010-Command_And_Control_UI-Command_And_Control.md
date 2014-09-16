#![](http://www.rpsgroup.com/images/2012-specific/RPSlogo.aspx) OOI Web UI Construction 
# Command and Control

| Use Case ID | 010 |
| --- | --- |
| Name | Command and Control |
| Scope of Work | Command and Control UI |
| Actors | Operator, Science, Facility |
| Requester | OL |
| Description | User executes steps to configure a platform or instrument (e.g., power on/off, set sampling rate, etc) |

## Definition

## Assumptions
- Operator has proper privileges for these operations
- All gliders and AUVs are commanded and controlled by the operator specific OMCs

##Scenarios 

    1. Mobile device A glider operator needs to change the sampling rate and dive pattern of a single glider to lower the overall power consumption to ensure that the glider has sufficient power to sustain a reduced mission until glider recovery. (This is not the typical, daily C2 required for normal mobile devices - but rather a major change.)

Steps
      1. It has been determined that the glider has insufficient remaining power to complete the mission without change.  It is decided to alter the flight pattern and dive sequence. 
      2. During normal daily operations the operator receives authorization and change instructions to make the glider changes.
      3. The operator logs into the vendor-provided glider pilot software.
      4. The operator prepares and tests the new mission profile for completeness and that it is within the safety parameters of the glider.
      5. The operator sends the command to the glider and awaits response.
      6. The operator receives glider response and monitors the mission.
      7. Automated emails are sent to individuals that have subscribed to events for this glider.
      8. The operator prepares and submits update notices for the OOI web page as needed.

    2. Cabled device The sampling rate for an instrument needs to be changed due to an underwater event of scientific interest. No 'return to previous rate' is anticipated in the short term.

Steps 
      1. Command and control for cabled devices (except for hydrophones, seismometers and perhaps cabled profilers) are via the UI of the OOINet.
      2. Through an established procedure, it is decided that a) an important event has occurred that justifies changing the current sampling strategy. In the case of a sudden "EVENT", the established procedure can allow a single operator to can make a unilateral judgment call on the sampling change, and then report the change in a follow-up notification and review meeting with otherstakeholders; b) the risk/feasibility analysis has been performed and shows the requested change both safe and achievable; and c) authorization should be sent from a Facility User to the Operator.
      4. The operator logs in to the UI.
      5. The operator prepares and tests the sampling rate change for completeness and that it is within the safety parameters of the platform and instrument.
      6. The operator sends the command to the instrument and awaits response.
      7. The operator receives platform/instrument response and monitors the rate change.
      8. Automated emails are sent to individuals that have subscribed to events for this instrument.
      9. The operator prepares and submits update notices for the OOI web page, as needed.

    3. Uncabled device Sudden EVENT The METBK package on a global mooring needs to be shut down because it sent an alarm of excessive power draw. 

Steps
      1. The operator on-call receives the alarm via cell phone while sleeping. 
      2. Recognizing this as an emergency event that risks the longevity and safety of the buoy, the operator logs into OOINet or OMC tools, quickly confirms the message and reads the emergency procedure associated with this alarm.
      3. Thereafter and based on the established procedure, the operator sends a preform 'shutdown' command to the METBK package via the OMC and Iridium. 
      4. Upon receipt of successful shutdown, the operator reviews the health and status of the other instruments/platforms on the mooring, logs the event, per procedure sends notice of event and action to a predetermined contact list, and creates a trouble report (TR).
      5. Upon arrival at work the next day, the operator reviews the alarm and operator actions with other OOI team members who have an interest in this occurance. Having determined that the data were valid and actions were correct, the operator is directed to edit the platform and package metadata to show the date/time of shutdown and to annotate why it was shutdown.
      6. The operator engineering team evaluates the data in detail and sends a requested update to the OOI web page describing the event, the actions taken, and plan going forward.
      7. The operator generates and sends an event report to OL.
      8. OL reviews the report and decide next actions.

## Comments
This UI contains the following:
- Status screens:
  - Port status and power information
    - Temperature
    - Current
    - Voltage

  - The abilitity to issue commands to the platforms
  - Port power control
  - Over-current limits
  - Platform state managemnt
  - Mission Executive
  - Event monitoring and status parameters
    - Status parameters come from the OMS

- Bridge the gap between the platform control and instrument management 
  - Immediately transition to instrument control from a platform/port page

- Port Schedules
- Events
- Wire-diagram that shows how the network is physically laid out.
