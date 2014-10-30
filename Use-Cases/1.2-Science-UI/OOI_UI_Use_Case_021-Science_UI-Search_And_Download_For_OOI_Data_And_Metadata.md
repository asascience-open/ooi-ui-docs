#![](http://www.rpsgroup.com/images/2012-specific/RPSlogo.aspx) OOI Web UI Construction 
#Search and Download for OOI data and metadata

| Use Case ID | 021 |
| --- | --- |
| Name | Search, Locate and download OOI data |
| Scope of Work | Science UI|
| Actors| Operator, External Science User |
| Requester | OL |
| Description| Allows subject, geographic or time-based search for OOI data based on specified criteria. |

##Definition

Science focused users need to find subject, space- or time-based data products from the OOI system, using search criteria they enter. Once the data is located (identified), users need to extract subsets from the located data, then download those data, unprocessed or processed, to local computer hard disk. The data is downloaded along with the associated metadata.

Examples of search 'subjects' include: facility (e.g., CGSN), platform (e.g., profiler, glider), measurement (e.g., temperature), instrument (e.g., ADCP).

For this use case, we use the following specific example: "A science user wants to examine the last two weeks of glider temperature profile data from the Ocean Station Papa".

##Assumptions

- A valid browser with high-speed internet connection is available and the CI can provide extracted data in a short time frame (seconds).
- The science user can, but does not have to be a registered user (i.e., the user can enter as a 'Guest') to browse, but must be a registered user to download.

##Scenario

The following steps describe how the actor might use the system to accomplish this task.

Steps:

1. The user enters the OOI system through a supported browser. The main data page appears with map and selection bar.
2. The user selects (by clicking) the area of interest (e.g., Ocean Station Papa) but there are other ways to search and select.
3. The user selects a platform of interest (e.g., mobile glider #1) from the map interface and the list of available data and data products appear. 
4. The user picks data or a data product of interest (e.g., temperature); However the user could select to download other data products (salinty, optical backscatter, chlorophyll fluorescence).
5. The selected data product(s) can then be visualized using the functions described in Use Case 003 (Graphing) or download and saved to the user's local computer disk if desired.
6. The download function will allow the user to select the time interval of interest, using the tool on the UI.
7. The user selects the download data option and specifies the desired data format.
8. The downloaded data will have all of the associated glider data (e.g., lat, long, depth) and desired sensor data product.
9. The user edits and uses the downloaded file.

##Comments

- This use case must take place within the User Interface of OOINet

