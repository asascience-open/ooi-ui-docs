#Steve Sizer System Review

All authentication and authorization will be controlled by us. Any request we make will be answered, therefore we must keep security in check.
The Command and Control plugin will be performed by Raytheon, but not in Omaha
 - Pete Cable - Raytheon out of San Diego - IDS
   - He has a demo for command and control
   - There is documentation on the wiki page - instrument driver control.
Web Services pipe over to our Status, C2, and Science
Asset management is a stand alone portion of uFrame
 - There will be a specific interface between asset management
Data managemnet has the L1 and L2 data product conversion
23 sensors are integrated. They can read and store a decent amount
 - They needed some asset and data management for some l1 and l2 parameters, but it is still a WIP.
 - Delivery 2 will have a more robust data management system - December 19th is next delviery and then mid Januray for the next
AWIPS uses several edex instances for different datasets to improve performance, balance the load, and keep data types seperate
The responsibility for security does not fall on uFrame.
uFrame might be holding our user database - roles, user, password, etc.
 - AWIPS already does this so maybe we can work this.  Chat with Everet about this.
THe L0 and L1 analytics are done in python
All python algorithms similar toADCPA
R9 is simply the name of their software drop.  Widgit framework - web based
Asset management contains the definition of object model and db structure with hard coded config files for delivery 1
QUESTION: Are we using R9?  
They are currently providing all the data on request.  They must slice the data. 
Redmine gant chart has their capabilities schedule as well as their percent complete.  This will be going public on Rutgers soon, but now it is just on locahost here in Omaha.  We can use this service to track their capabilities for us to leverage.



##Wifi Credentials
pass: qNkz35
user: dmaher01


