#![](http://www.rpsgroup.com/images/2012-specific/RPSlogo.aspx) OOI Web UI Construction 
#Compare Data from Different Sensors

| Use Case ID | 034 |
| --- | --- |
| Name | Compare Data from Different Sensors  |
| Scope of Work | Science UI|
| Actors | Science, Data manager, Data evaluator  |
| Requester | OL |
| Description | User configurable capability to display side by side measurements from different instruments and/or systems for cross comparison. |

##Definition

The system provides the user the ability to display multiple measurements from different instruments and/or systems for cross comparison.

##Assumptions

- Includes visualization of time series, profiles, tracks, images, and other date types.
- There will be an ability to set a default visualization plot

##Scenario
User wants to display temperature data from different sensors in different locations

 1. User searches for first temperature time series data that they wish to compare.
 2. User selects the "compare" option.
 3. User searches for and selects second data product of interest for a specific location and time.
 4. User selects the quickplot desired: time series, profile, etc.
 5. System displays the time series overlayed in one graph.
 6. The X and Y Axes can be rescaled if so desired by the user.


User wants to display two different types of data from disfferent sensors in the same location.
 1. User searches for first temperature  and chlorophyll fluorescence time series data that they wish to compare.
 2. User selects the "compare" option.
 3. User searches for and selects second data product of interest for a specific location and time.
 4. User selects the quickplot desired: time series, profile, etc.
 5. System displays the data overlayed in one graph, with an  axes (user specified X or Y) for the each specific data product.
 6. The X and Y Axes can be rescaled if so desired by the user.



