#![](http://www.rpsgroup.com/images/2012-specific/RPSlogo.aspx) OOI Web UI Construction 
# Map Overlays

| Use Case ID | 006 |
| --- | --- |
| Name | Map Overlays |
| Scope of Work | Science UI |
| Actors | Science, Facility, Operators |
| Requester | OL |
| Description | Support layering of environmental data  |

## Definition
Allow for the Layering of environmental data (2d fields, wind, waves, currents, temp, altimetry, etc.). 
## Assumptions

## Scenario
The standard map used in the interface should be able to include overlays.  Stock overlays will be provided (e.g. HYCOM, current weather).  Users may add their own layers through WMS endpoints or tile servers.

Science user wants to compare a sea surface temperature model to the actual measured values by the Pioneer Array
1. A Science user wishes to overlay a sea surface temperature model over the Pioneer Array region.
2. The user goes to the science UI and is provided a method of overlaying the SST model.
3. When accessing the temperature data from the Pioneer array, the user is given the option of comparing the values against the model overlayed on the map.

An operator wants to view the weather over the EA Array to see if a storm could be the possible reason for a lack of connectivity to an asset.
1. Operator goes to the science page and finds the asset of conern.
2. Operator uses the UI to overlay the current percipitation and cloud coverage over the area.
3. Operator determines stormy conditions are likely raising the sea state, causing intermittent or no connectivity for the instrument.
4. Operator files an action item for someone to check on this instrument and the weather a short time in the future to make sure connectivity returns after the storm is gone.


