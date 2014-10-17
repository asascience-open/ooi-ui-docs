Background:

- Asset/Property management information is maintained in the system as linked
  lists of metadata parameters.
- Two broad classes of elements (generic term from the data model for physical
  assets) are tracked, logical and physical.
- A physical element is something like an instrument. A physical element would
  be defined by a list of parameter-value pairs. For example, an instrument
  would be defined by OOI property number, six letter code, English language
  displayable name, manufacturer model number and revision number, software
  version number, serial number, responsible IO property number, location,
  condition/state, etc.
- A logical element is something like a specific deployed platform. This is a
  logical element because it represents a logical entity that is implemented at
  any given time by a specific set of physical elements, but these physical
  elements are periodically replaced. The platform logically exists at all
  times, but the physical implementation will change periodically. These
  logical elements are defined by a list of parameter-value pairs. In this
  case, the list includes a reference designator, OOI part number, responsible
  IO part number, a list of all physical elements used to implement the logical
  element (probably the OOI property number and serial number of each item),
  etc.
- The parameter lists associated with an entity include some parameters that
  change with time and others that don’t. For example, an instrument serial
  number does not change, but associated calibration parameters do change.
  Similarly, for a logical platform, the reference designator does not change,
  but nearly everything else about it does change periodically.
- To deal with this time variability, the data structure defining each element
  in the database has an associated event log. When an event takes place that
  changes a parameter, an entry is added to this log and the associated
  parameters are changed. For example, when an instrument is re-calibrated, a
  “calibration” event is logged and the calibration parameters for that
  instrument are updated with a new value and effective date.
- In the above example, the definition of the physical instrument maintains a
  list of the calibration parameters as they change over time. The same is true
  for all other time varying parameters for all elements. Note that the serial
    numbers of instruments installed on a logical platform are time varying and
    they change when a “deployment” event is logged for that logical platform.
- When a user requests data for a specific instrument type on a specific
  logical platform for a specific period of time, an associated data query is
  submitted to the database/data management system. The data management system
  will then look at the definition of the logical platform, pull up the serial
  number or numbers for the specified instrument type (the time span may cross
  deployment boundaries). This will be a list of serial numbers and associated
  effective dates. Now the system will look at the physical instrument records
  for the identified instruments by serial number for the specified date
  ranges. The required calibration parameters are each listed as time varying
  lists. The appropriate parameter values will be pulled as needed to cover
  the specified time frame. The end result is that for each calibration
  parameter we will have a list of parameter values that change over time.
  This list is passed to the data processing algorithm along with science
  data to be processed that have been similarly collected via a database
  query.

Assumptions:

- At least one round of metadata entry has been completed to define the initial
  deployment of each logical platform. The first instance metadata collection
  and entry into the system database will likely be a relatively ugly, trial
  and error process of determining what parameters are important and how they
  are linked to each other. However, the general principles are clear as
  described above and in the strawman data model. In the end we are just
  defining a series of linked lists of parameter-value-date/time triplets. This
  will be tedious but it is not logically difficult.

Notes:

- For each of the scenarios described below, while the specific list of
  parameters and the specific menu/pull-down options vary from one hardware
  element and event type to others, the basic process and the basic structure
  of the Asset Management user interface do not change. In all cases, the user
  is presented with a list of parameter-value-time/date triplets associated
  with the hardware element and a set of available event types to record. A
  relatively simple and logically consistent user interface should be possible.

Metadata Change:

- An instrument that is already in the property management database has been
  returned from a vendor after being refurbished and recalibrated after return
  from a deployment. The vendor has provided printed calibration sheets for the
  instrument.
- A properly authorized user wants to enter the calibration data into the
  system.
- The user logs into the OOI system and opens the Asset Management user
  interface.
- The user requests, via a series of pull-down menu selections, the specific
  instrument data record based on sensor type and serial number.
- The user is presented with a list of parameter-value pairs associated with
  that instrument.
- The user selects “Calibration” from a pull-down list of defined event types
  and enters an effective date-time.
- The user changes the several calibration parameters from previous values to
  new values.
- The user reviews the changes and submits the change for processing.
- The data management system logs the calibration event in the instrument data
  record and adds the new calibration parameters, and the associated effective
  date, into the parameter records for this instrument.

 
Platform Deployment:

- Sometime well in advance of actual deployment, a properly authorized user
  wants to define a new physical instance of a logical platform for deployment.
- The user logs into the OOI system and opens the Asset Management user
  interface.
- The user requests, via a series of pull-down menu selections, the specific
  platform she wants to update.
- The user is presented with a list of parameter-value pairs associated with
  that logical platform.
- The user selects “Create New Instance” from a pull-down list of defined event
  types and enters an effective date-time. Since the effective date is in the
  indeterminate future, a null value is entered (this will be changed to a real
  date-time when the new platform is actually deployed).
- The user changes the many parameters from previous or null values to new
  values. This includes serial numbers of instruments and other components to
  be installed on the physical platform and the unique serial number of the
  to-be-deployed physical platform.
- The user reviews the changes and submits the change for processing.
- The data management system creates a new physical platform instance,
  associates this physical instance with the logical platform type, assigning a
  null effective date, and logs the event in the logical platform data record
  event log.

Failure Event:

- A properly authorized user has identified an instrument failure in bench
  testing.
- The user logs into the OOI system and opens the Asset Management user
  interface.
- The user requests, via a series of pull-down menu selections, the specific
  instrument data record based on sensor type and serial number.
- The user is presented with a list of parameter-value pairs associated with
  that instrument.
- The user selects “Failure” from a pull-down list of defined event types and
  enters an effective date-time.
- The user is presented with a set of fields to define the failure type and
  equipment disposition.
- The user enters a brief description of the failure in the “Notes” parameter.
- The user changes the “State” parameter to “Failed” and the “Location”
  parameter to “Vendor”.
- The user reviews the changes and submits the change for processing.
- The data management system logs the failure event in the instrument data
  record (this failure in the log supports periodic review and reporting of
  failure rates), changes the instrument state and location appropriately, tags
  the changed parameters with the effective date, and updates the parameter
  records for this instrument.

