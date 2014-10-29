#![](http://www.rpsgroup.com/images/2012-specific/RPSlogo.aspx) OOI Web UI Construction 
# Graphing

| Use Case ID | 003 |
| --- | --- |
| Name | Graphing |
| Scope of Work | Science UI |
| Actors | Science User |
| Requester | OL |
| Description | Different graphs desired for displaying data |

## Definition
Several different graph types are desired to visualize data collected by OOI infrastructure by an external science user.

## Assumptions
Use case for searching described elsewhere. Expect that the user will have a spatial frame of reference available while viewing data products (desirable to have, not need to have). Expect that the x-axis will default to time. 

## Scenario 1. A science user wants to create a graph to visualize data across the entire OOI.
1. Science user searches for and selects the instrument (e.g., CTD) and/or measurement of concern.
2. Science user selects the type of graph to be created based on need. The graph options the user may select:
  a. Shall have the ability to plot an x-y plot with the user selecting the variable (depth, time, data product) for the x and y-axis.
  b. Shall, as above for x-y-z plots allowing the user to choose each of the axis (depth, time, data product)
  c. Will allow multiple data products to be plotted on the x-axis with a single y-axis.
3. User may select filters based on
  a. Time
  b. Depth
  c. Spatial (lat & long)
  d. data product maximum and minimum
4. User requests the plot and is provided with the desired graph. Individual parameter values are displayed when hovering over the plotted line.
5. User may go back to adjust the boundings for a better fit or scaling.
6. User may save plot as a picture along with the data table.



