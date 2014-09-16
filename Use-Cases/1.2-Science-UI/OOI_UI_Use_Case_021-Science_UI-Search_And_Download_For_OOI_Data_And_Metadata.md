#![](http://www.rpsgroup.com/images/2012-specific/RPSlogo.aspx) OOI Web UI Construction 
#Search and Download for OOI data and metadata

| Use Case ID | 021 |
| --- | --- |
| Name | Search, Locate and download OOI data |
| Scope of Work | Science UI|
| Actors| Science |
| Requester | OL |
| Description| Allows subject, geographic or time-based search for OOI data based on specified criteria. |

##Definition

Science focused users need to find subject, space- or time-based data products from the OOI system, using search criteria they enter. Once the data is located (identified), users need to extract subsets from the located data, then download those data, unprocessed or processed, to local computer hard disk.

Examples of search 'subjects' include: facility (e.g., CGSN), platform (e.g., profiler, glider), measurement (e.g., temperature), instrument (e.g., ADCP).

For this use case, we use the following specific example: "A science user wants to examine the last two weeks of glider temperature profile data from the Gulf of Alaska region"

##Assumptions

- A valid browser with high speed internet connection is available
- The science user can, but does not have to be a registered user (i.e., the user can enter as a 'Guest')

##Scenario

The following steps describe how the actor might use the system to accomplish this task.

Steps:

1. The user enters the OOI system through a supported browser. The main data page appears with map and selection bar.
2. The user selects (by clicking) the area of interest (e.g., highlighted box in Gulf of Alaska) (there are other ways to search and select)
3. The user selects a platform of interest (e.g., mobile glider #1). A list of available data and data products appear 
4. The user picks data or a data product of interest (e.g., temperature). A 'strip' chart of temperature appears
5. The user selects the time interval of interest, using the tool on the UI.
6. The user 'clicks' on the download button. (Depending on the browser being used, a table or 'tab' will appear on the screen. The user opens this object and an Excel table appears on the screen. Using MS Excel, the user saves to their local computer disk
7. The user edits and uses the downloaded file.

##Comments

- This use case must take place within the User Interface of OOINet

