#![](http://www.rpsgroup.com/images/2012-specific/RPSlogo.aspx) OOI Web UI Construction 
#Examine a data product or auxiliary (i.e. engineering) data 

| Use Case ID | 025 |
| --- | --- |
| Name | Examine a data product or auxiliary (i.e. engineering) data  |
| Scope of Work | Science UI|
| Actors | Any registered science user; ex-PI, MIO-SU |
| Requester | OL |
| Description | User performs analysis on data set to determine if it is of sufficient quality to use in research. |

##Need Statement
A user is conducting a regional analysis in the NE Pacific of annual variability of upper ocean chlorophyll fluorescence, using data from ships of opportunity, OOI moorings and gliders, and remotely-sensed ocean color. The user needs to confirm that the chlorophyll data products (2015-2017) from the selected OOI instruments on mooring and gliders are acceptable for inclusion in this regional data analysis.

##Definition

Science Justification for this use case: before inserting the OOI data from 2015 - 2017 into the larger scale regional analysis, the authorized user must be confident that the OOI data is internally consistent across multiple deployment cycles, and that the data quality is understood. The user (in this case an authorized user- e.g., OOI Ps) will examine the OOI automated Data QC results and may also wish to apply alternative QC protocols to compare the results across the successive deployment cycles. The results of these analyses may be useful to other OOI users, so the user wishes to provide his/her analyses for examination by others.


##Assumptions

- Includes visualization of time series, profiles, tracks, images, and other date types.
- More than one year of OOI chlorophyll fluorescence data has been obtained from fluorometers on the moorings and gliders at Station Papa, on the cabled profilers at Axial, Hydrate, and on the moorings, profilers, and gliders within the Endurance Array.
- The regional data analysis will be conducted outside the OOI Net software environment.


##Scenario
(will limit the scenario to just one of the relevant chlorophyll fluorescence instruments. There are dozens of fluorescence instruments within the OOI domain in the NE Pacific. The steps to complete the scenario would be the same for each of these instruments or platforms.)

Steps:

1. Search and download the chlorophyll data product from 5m below the surface on the Surface Mooring at the mid-shelf WA site, 80m water depth (reflected in SciUser.1);
2. Retrieve & download all QC information on that data product over the 3 year history (This is accomplished as part of the data time-series download);
3. Search and download metadata related to that product (calibration history, serial #, instrument deployment history, etc)
4. Outside OOI Net, user evaluates consistency of chlorophyll product across the deployment boundaries, comparing product time series to supplemental data records (time series) from remote sensing or other research expeditions;
5. Based on comparison with other data sets, user decides to apply (outside of OOI Net) an alternative method for trend correction (instrument drift or biofouling) within each 6-month deployment interval within the time series;
6. Authorized user (only MIO-SU) submits to the OOINet system- revised data created externally with HITL processing and any additional external information for other users 

User annotates the data product (comments, alternative processing steps, etc)


