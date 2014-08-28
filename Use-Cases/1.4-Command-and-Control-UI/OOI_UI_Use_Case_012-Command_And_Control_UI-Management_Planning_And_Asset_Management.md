#![](http://www.rpsgroup.com/images/2012-specific/RPSlogo.aspx) OOI Web UI Construction 
# Management Planning and Asset Management

| Use Case ID | 012 |
| --- | --- |
| Name | Management Planning and Asset Management          |
| Scope of Work | Command and Control UI |
| Actors | Observatory Director, O&M Leads, marine operators |
| Requester | OL |
| Description | User executes steps to load a different configuration (sensors, platforms) into the OOI database as a result of new deployments or repairs. User executes steps to sustain the approved configuration. |

##Definition
Management Planning and Asset Management allows for establishing / altering / maintaining the configuration of OOI assets, including instruments, platforms, primary and secondary infrastructure, and shore-side hardware and software.


##Assumptions
- Includes registration, asset tracking, calibration information, etc.
- An asset tracking system is a functional component of OOI Net.
- Operators have command and control capability (demonstrated via Operator Case #1).

##Scenario


The marine operator must execute a 'turn' of the Pioneer Array in April 2015. This will involve the recovery of five Wire-Following Profiler moorings, three Coastal Surface moorings, two Coastal Surface Piercing Profiler moorings, two AUVs, two AUV docks, and six coastal gliders. The cruise will also redeploy new or refurbished versions of those same moorings and platforms. The 'pre-April' configuration of all these moorings and platforms has been stored in the asset tracking module of OOINet. At the completion of the 'turn', the asset distribution within the Pioneer Array must be incorporated into the asset tracking module. The metadata tables for each of the recovered and deployed items also must be edited and saved to reflect the new configuration.

STEPS (selecting 1 Coastal Surface mooring as a representative example)

1. Establish During pre-deployment integration and burn-in, the operator builds (edits) the 'Array preload' template, inserting all required information (see requirements for Asset Tracking 'load' process) into the template for each element (instrument, riser cable, buoy hull, etc) of the asset tracking system. 
2. Quality control staff validates the accuracy of the information in the template.  
3. If no alteration of configuration while at sea, approved configuration file uploaded to CI upon return from cruise, with CI acknowledgement of receipt. 
4. CI conducts validation testing of the new load into the asset tracking database.
5. Upon completion of validation testing, CI O&M Lead provides notification to OOI Director that the updated of the Asset Tracking Database is now functional within OOI Net.
6. New configuration, including new metadata (new calibrations, new instrument serial #s, etc), incorporated into the documentation page(s) of OOINet (see Ops Use Case #6).
7. Alter before completion of deployment If any assets fail pre-deployment testing and are replaced with spares, the required information for the spare is entered into the template, replacing the instrument previously used. Revised pre-load file now pending PM sign-off.
8. Upload The approved configuration file is submitted to CI for ingestion into OOI Net, with CI acknowledgement of receipt.
9. CI conducts validation testing of the new load into the asset tracking database. 
10. Upon completion of validation testing, CI O&M Lead provides notification to OOI Director that the new instance of the Asset Tracking Database is now functional within OOI Net. 
11. New configuration, including new metadata (new calibrations, new instrument serial #s, etc), incorporated into the documentation page(s) of OOI Net (see Ops Use Case #6).
12. Alter configuration during deployment Operator, in response to alert about excessive humidity in DCL#2 on the central Surface Mooring, takes DCL#2 and associated instruments off-line by sending 'off' command(s) to the DCL. 
13. New configuration, including new metadata (new calibrations, new instrument serial #s, etc), incorporated into the documentation page(s) of OOI Net (see Ops Use Case #6).
14. Maintain configuration of the OOI Operator uses information in the configuration file, in conjunction with SOPs (under development), to sustain the OOI configuration of assets between deployment and recovery cruises


The Management Planning and Asset Management provides the suer with the following:
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