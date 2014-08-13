 Scope

 - About 6 people specifically acting as operators and routine monitoring

Types of moorings:
 - Fixed Platforms, Surface Moorings
  - 3-10 Controller (A few hundred parameters)
  - Example: [CG_STC_ENG IDD](https://confluence.oceanobservatories.org/display/instruments/cg_stc_eng_stc)
 - Fixed Platforms, Wire Following Profiler
  - Single Controller
 - Glider Assets (Mobile Assets)
 - AUV
  - When it's in the dock, that's when the status is focused on.

## General Comments

 - Instruments ordered by their position in the water column
 - Be able to see the asset metadata associated with instruments and platforms
 - Marine operator handoff:
   - Clear transfer of information between operators.
   - Who did what
   - What actions were taken
   - What actions are pending
   - Escelation of problems or notifications
   - A log currently in use, e-logs (OSU)
 - Asset Management: Assets having user annotations
 - Physically see where the ship is.

  
## Surface Moorings

#### Interesting Elements

Surface Moorings Telemetry:
 - Scheduled
 - Backups
 - Emergency

Telemetries Schedules:
 - Does it keep schedule
 - Is it behind or using backup telemetry system
 - Call Logs

Most of the information we want comes out of some key status files. One of them is the system log, a syslog file. It's generated and sent basically during a telemetry session. There should be one every single day for some of the moorings. 

The system log for the surface moorings is an aggregation of many different elements within the mooring.
 - Information about hte telemetry
 - Port status
 - DCL
 - Supervisor on the surface mooring
 - Lists of information that was sent in the last telemetry
 - CPM Status Lines

#### Main Concerned

Tiers: See the presentation

Tier 1: Big picture
Tier 2: Easy to see the subsystems
Tier 3: 

Spot a lot of trend analysis by eye.
Example: 
 - Humidity on a DCL sensor over a long time scale.
 - Potential Fail Candidates to drive trend analysis use cases.


One other log would be extremely relevant
A description for all the elements.
There are log files that are on the mooring that are not regularly sent.


#### Workflows

 - Top to bottom, following a checklist.
 - 

## Profiler Mooring

- Status log every telemetry session



