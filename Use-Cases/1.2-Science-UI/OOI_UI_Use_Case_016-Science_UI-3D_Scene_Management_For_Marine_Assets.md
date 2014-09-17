#![](http://www.rpsgroup.com/images/2012-specific/RPSlogo.aspx) OOI Web UI Construction 
# 3D Scene Management for Marine Assets

| Use Case ID | 016 |
| --- | --- |
| Name | 3D Scene Management for Marine Assets           |
| Scope of Work | Status UI |
| Actors | Operator, Facility, Science |
| Requester | RSN |
| Description |  |

## Definition
Display a 3D scene for the marine assets to assist operators in visualizing and quickly identifying faults in the infrastructure.

## Assumptions
- Assets have associated 3d models that can be downsampled (reduce vertices from many to few)

## Scenario

The user has a 3D rendering of the marine assets and surrounding area so that they can identify any possible issues that arise. 

1. The operator recieves an alert warning them that an asset is no longer providing data.  
2. The operator opens the 3D scene management for that asset.
3. The oeprator notices that the mooring is designed for a 200m water depth, but the deployed area is 500m.
4. The operator files a Trouble Ticket to fix this issue.
