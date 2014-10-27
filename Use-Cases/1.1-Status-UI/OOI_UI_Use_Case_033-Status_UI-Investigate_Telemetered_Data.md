#![](http://www.rpsgroup.com/images/2012-specific/RPSlogo.aspx) OOI Web UI Construction 
#Investigate Telemetered Data

| Use Case ID | 033 |
| --- | --- |
| Name | Investigate Telemetered Data |
| Scope of Work | Status UI |
| Actors: | Data Manager, Marine Operators, Science, Facility, OL |
| Requester | OL |
| Description: | Data Manager receives 'trouble report' and must investigate  |


##Definition

There will be frequent and sometimes confusing reports of 'problems with the data.' It is the role of the Data Manager to assume the role of 'end-to-end' data detective to investigate the report. If the report is valid, it is the DMs responsibility to orchestrate and then monitor the correction. Plus, the DM must keep the community informed of this and all other data related issues.

##Assumptions :

- System was working as accepted

##Scenario

  1. The DM receives a TR from an external source that there is no data from the Pioneer Inshore Upstream WFP after May 29, 2014.
    1. The DM uses the public UI to view the current data from this source and confirms the report.
    2. The DM views the data logs to verify last time of data acquisition by the: CyberPop, the OMC, and the satellite downlink site.
    3. The DM views the status of the communications pathway from the OMC to the CI and verifies 'OK'
    4. The DM checks the data path processes at the CyberPop and verifies them 'OK'.
    5. The DM checks the OMC status and verifies 'OK'
    6. The DM injects a test particle into the OMC/CI server and it properly progresses through the system. 
    7. Having isolated the problem upstream of the OMC server, the DM contacts the O&M Lead for Pioneer and transfers ownership of the TR.
    8. The O&M Lead investigates and fixes the problem (finds that the data have been mistakenly rerouted to a null address)
    9. The O&M Lead completes the TRE and sends ownership back to the DM.
    10. The DM validates that data are now flowing, informs the community and reporter of the problem of the issue/fix, and closes the TR

  2. The DM receives a TR that there is a large gap in a deployed seafloor hydrophone and wants to know where to acquire the data.
    1. The DM uses the standard UI to confirm the data gap and begins the investigation.
    2. Knowing that the hydrophones are a Tier 1 instrument, the DM suspects deliberate diversion/blockage by the Navy.
    3. The DM first checks the status OMC and CI servers to rule out communication or storage problems; they are ruled out.
    4. The DM then contacts the Navy POC but receives a rather standard response, deliberately constructed to neither confirm nor deny and Navy activity wrt this dataset.
    5. The DM responds to the TR with a prepared response stating that our system appears to be working but that as a Tier 1 instrument, the daya may be going under review.  The TR is closed. 
