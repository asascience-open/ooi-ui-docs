#![](http://www.rpsgroup.com/images/2012-specific/RPSlogo.aspx) OOI Web UI Construction 
# Infrastructure Asset Management

| Use Case ID | 001 |
| --- | --- |
| Name | Infrastructure Asset Management |
| Scope of Work | Asset Management UI |
| Actors | Operator, Facility |
| Requester | OL |
| Description |  |

## Definition

## Assumptions
- Database that contains a comprehensive structure to describe and document the marine infrastructure:
  - Reference Designator
  - Array -> Platform -> Site -> Port -> Instrument
- The asset spreadsheet template is defined and mapped to the data model.


## Scenario
A facility user wants to add 50 new assets to their OOI array
1. User loads all of the information into a spreadsheet.  This spreadsheet must be preformatted.
2. User navigates to the Asset Management UI and goes to 'Load new assets'
3. User is provided a prompt where they can naviagte to the spreadsheet and select it.
4. User porivdes metadata about the load.
5. Asset Management UI attempts to injest these assets into the Asset Management database.
6. If the injestion fails, the UI provides details of the failure to the user.
7. If the injestion successfully sompletes the user is notified.

A facility user wants to edit an asset.
1. User navigates to the asset in the Asset Management UI.
2. User views the asset metadata.
3. User selects 'edit' and edits the metadata as desired.
4. User selects 'save'.  UI attempts to update the data model with these changes.
5. If the injestion fails, the UI provides details of the failure to the user.
6. If the injestion successfully sompletes the user is notified.

A facility user wants to delete an asset
1. User navigates to the asset in the Asset Management UI.
2. User views the asset metadata.
3. User selects 'delete'.
4. User is prompted whetehr they are sure they want to delete asset.  User selects that yes they are sure they want to delete the asset.  UI attempts to update the data model with this asset deletion.
5. If the injestion fails, the UI provides details of the failure to the user.
6. If the injestion successfully sompletes the user is notified.


