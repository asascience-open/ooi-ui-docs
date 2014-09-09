#![](http://www.rpsgroup.com/images/2012-specific/RPSlogo.aspx) OOI Web UI Construction 
#CI Status

| Use Case ID | 036 |
| --- | --- |
| Name | CI Status |
| Scope of Work | Status UI |
| Actors: | Data Manager (DM), O&M Leads, O&M engineers |
| Requester | OL |
| Description: | Display that status of the Cyber Infrastructure for OOI |


##Definition
If there is ever a gap in the reporting of data, it would be helfpful for the diagnosing actor to determine if the issue resides in the instrument or in the CI. 

##Assumptions :


##Scenario
This scenario is taken from [OOI Use Case 033 - Status UI - Investigate Telemetered Data](OOI_Use_Case_033-Status_UI-Investigate_Telemetered_Data.md).  It is slightly altered to explain the Status UI better.
  1. The DM receives a TR from an external source that there is no data from the Pioneer Inshore Upstream WFP after May 29, 2014.
    1. The DM uses the public UI to view the current data from this source and confirms the report.i
    2. The DM views the data logs to verify last time of data acquisition by the: CyberPop, the OMC, and the satellite downlink site.
    3. The DM opens the CI/DM screen.
        a. The CI/DM screen shows a list of all assets.  This list is can be searched, filtered, and sorted by asset name, ID, array, and platform.  
        b. Upon slecting an asset, the DM can open the network topology map showing the communications pathway for this specific asset.  
            i. The network topology map is colored per status (stoplight coloring scheme)
    4. The DM observes the status of the communications pathway from the OMC to the CI and finds it 'green'
    5. The DM uses the CI screens to check the data path processes at the CyberPop and finds them 'green'.
    6. The DM checks the OMC screens and they show 'green.'
    7. The DM injects a test particle into the OMC/CI server and it properly progresses through the system. 
    8. Having isolated the problem upstream of the OMC server, the DM contacts the O&M Lead for Pioneer and transfers ownership of the TR.
    9. The O&M Lead investigates and fixes the problem (finds that the data have been mistakenly rerouted to a null address)
    10. The O&M Lead completes the TRE and sends ownership back to the DM.
    11. The DM validates that data are now flowing, informs the community and reporter of the problem of the issue/fix, and closes the TR

