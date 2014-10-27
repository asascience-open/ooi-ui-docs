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
- The user has logged into the User Interface and has privileges to create/edit/delete resources and corresponding metadata.


## Scenario
Example 1) A facility user wants to add 50 new assets to their OOI array
1. User enters all of the information into a spreadsheet.  This spreadsheet must be preformatted with required fields.
2. User navigates to the Asset Management UI and selects the option to 'load new assets'
3. User is provided a prompt where they can naviagte to the spreadsheet and select it.
4. User Interface prompts the user for required metadata about the new assets. (may be included in preformatted spreadsheet)
5. Asset Management UI attempts to injest these assets into the Asset Management database.
6. If the injestion fails, the UI provides details of the failure to the user.
7. If the injestion successfully completes the user is notified. The user may navigate back to the Asset Management UI search window and enters a newly ingested asset. New asset is displayed with corresponding metadata.

Example 2) A facility user wants to edit an asset.
1. User navigates to the asset in the Asset Management UI.
2. User views the asset metadata.
3. User selects the option to 'edit' and edits the metadata field(s) as desired.
4. User selects the option to 'save'.  UI attempts to update the data model with these changes.
5. If the injestion fails, the UI provides details of the failure to the user.
6. If the injestion successfully completes the user is notified. Updated metadata value is displayed.

A facility user wants to delete an asset
1. User navigates to the asset in the Asset Management UI.
2. User views the asset metadata.
3. User selects the option to 'delete'.
4. User is prompted whether they are sure they want to delete asset and displayed related artifacts that will be deleted.  User selects that yes they are sure they want to delete the asset.  UI attempts to update the data model with this asset deletion.
5. If the deletion fails, the UI provides details of the failure to the user.
6. If the deletion successfully completes the user is notified. Deleted asset is no longer displayed and cannot be searched for.


