#![](http://www.rpsgroup.com/images/2012-specific/RPSlogo.aspx) OOI Web UI Construction 
#Annotate Data

| Use Case ID | 024 |
| --- | --- |
| Name | Annotate Data |
| Scope of Work | Status UI |
| Actors: | Operators, PSs |
| Requester | OL |
| Description: | It permits two levels of data annotation. The first is a general capability open to all registered users. It allows the registered user to add text, including URLs to comment fields of data products. This permits the community to share their results, observations, concerns and questions about a particular data set.The second level is for authorized users only- mostly OOI operators and/or PSs. This requires special permissions and allows annotation of items like data quality, mission status, and other 'official' comments/documentation. |

##Need Statement
Data sets must be capable of being annotated to contain both observations by the end users and 'official' comments relating to availability, problems with the data, corrections that have been made, etc.

##Definition

The OOI provides a free form text capability for the two identified groups to annotate: data values, data periods, entire streams, entire platforms, entire sites, and entire arrays.

##Assumptions

- The OOI supports at least two permission levels of annotation
- Annotation may be either data cell specific or time period specific or data set in general.


##Scenario
A registered user (scientist at ONC) is reviewing the data from the Washington line and notices an unusual set of CDOM values. Realizing this might be of scientific interest, she wants to annotate the product and site metadata.

STEPS:

1. The scientist is examining the data and determines the above feature as scientifically interesting.
2. The scientist examines other data (other sensors, engineering data) and decides it is likely a real event.
3. The scientist opens the "annotate and report event" screen.
4. It is automatically prefilled with user information (name, email, phone, etc). The user completes the rest of the form by selecting the time period, location, platform, product, and typing in the free form comments.
5. The user also selects the "SUSPECTED EVENT" and submits
6. By selecting SELECTED EVENT, the system sends an alert to the MIO operator and to the PS responsible for the CDOM
7. The annotated data product is available for others to read or add additional comments.
