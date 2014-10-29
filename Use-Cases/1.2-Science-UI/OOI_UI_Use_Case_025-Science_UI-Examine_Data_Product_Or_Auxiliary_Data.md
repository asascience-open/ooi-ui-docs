#![](http://www.rpsgroup.com/images/2012-specific/RPSlogo.aspx) OOI Web UI Construction 
#Examine a data product or auxiliary (i.e. engineering) data 

| Use Case ID | 025 |
| --- | --- |
| Name | Examine a data product or auxiliary (i.e. engineering) data  |
| Scope of Work | Science UI|
| Actors | Operator, Data Manager, Science |
| Requester | OL |
| Description | User performs analysis on data set to determine if it is of sufficient quality to use in research. |

##Need Statement
A user is conducting a regional analysis of annual variability of upper ocean chlorophyll fluorescence, using data from ships of opportunity, OOI moorings and gliders at the Pioneer Array. The user wants to compare ship data collected during the pioneer array deployments with the OOI in-water assests. The user needs to confirm that the chlorophyll data products (2015-2017) from the selected OOI instruments on mooring and gliders are acceptable for inclusion in this regional data analysis.

##Definition

Science Justification for this use case: before inserting the OOI data from 2015 - 2017 into the larger scale regional analysis, the authorized user wants to be confident that the OOI data is internally consistent across multiple deployment platforms, and that the data quality is understood. The user (in this case an authorized user) will examine the OOI automated Data QC results and may also wish to apply alternative QC protocols to compare the results across the successive deployment cycles. The results of these analyses may be useful to other OOI users, so the user wishes to provide his/her analyses for examination by others.


##Assumptions

- Includes visualization of time series, profiles, tracks, images, and other date types.
- More than one year of OOI chlorophyll fluorescence data has been obtained from fluorometers on the moorings and gliders at the Pioneer Array.
- The data collected by the ships is inserted into the OOI Infrastructure.


##Scenario 1
(We will limit the scenario to just one of the relevant chlorophyll fluorescence instruments. There are dozens of fluorescence instruments within the OOI domain of the Pioneer Array. The steps to complete the scenario would be the same for each of these instruments or platforms.)
1. Authorized user logs in and goes to the Pioneer web page.
2. Search and download the chlorophyll data product from moored and glider data from a specific depth range and for a specific time range when the ships are present in the Pioneer Array.
3. The displayed data product(s) may be visualized using the functions described in Use Case 003 (Graphing) or downloaded and saved to the user's local computer disk if desired.
4. Search and download all QC information on that data product over the 3 year history (This is accomplished as part of the data time-series download) with all required associated data (depth, lat, long) with each of the platforms.
5. Search and download metadata related to that product (calibration history, serial #, instrument deployment history, etc)
6. User does a search for the ship data for a specific time range and location.
7. The displayed data product(s) may be visualized using the functions described in Use Case 003 (Graphing) or downloaded and saved to the user's local computer disk if desired.
8. User compares data on their computer and the results suggest a drift in the data.
9. Authorized user submits findings to the OOINet administrator via trouble ticket system.
10. OOINet administrator takes action on the trouble ticket.



