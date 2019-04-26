# DataDive Project Outline for Audubon Society 
The DataDive will be assisting the Audubon Society to build off of existing coastal erosion work to solutionize their research on habitat destruction in preparation for the coming hurricane season. 
Background
DataKind will be working with the Audubon Society to solutionize the work done on the Rapid Evaluation of Coastal Habitat Change Report into a solution that can be used in the 2019 hurricane season. 

Our goal is to be able to say:  “After this most recent Hurricane, <X> amount of beaches were flooded and <Y> amount of Marshes were flooded. 
Here is where they are <Insert List or Map> “

## Team
Data Ambassadors - Ren C’deBaca (rectheworld@gmail.com) and David
Project Partners - Kathy 
Slack channel - https://dkdc.slack.com/messages/CFLS9925S/? 


## Problem / Impact Statement
I want to use Satellite data to assess the extent of flooding so that the Audubon Society can assess bird habitat destruction so that conservation efforts can be more targeted. 

## Available Datasets
After discussions with the Audubon Society and assessing the data available, the primary source of satellite data and band will be Sential-2. 

Information about Sentinel-2 data and how to work with it in python is available here: 
	Sign up for a free trial here
https://services.sentinel-hub.com/oauth/subscription
NOTE: we will be useing eo-learn package to interface with sentinel-2

The area of Interest will be the same as the Area of interest in the original report. A shapefile of the AOI is available here:
https://drive.google.com/open?id=1j-7OrGPgjQ2WTADqIfgi_raz09nxfwET

Support Shapefiles from Audubon (These are the shapefiles that were used or produced in the Rapid Evaluation of Coastal Habitat Change) 
https://drive.google.com/open?id=1j-7OrGPgjQ2WTADqIfgi_raz09nxfwET

Tidal Data
www.tides4fishing.com

## Project Phases
Project phases should be updated to fit the needs of the specific project, but a list of standard phases would be:

- Introduction: Brief on Project Goals and Intro to working with Satellite Data
- Use NDVI to determine if flooding has occured within an example DemoZone.
- Design and Implement a system where pre-hurricane data can be collected, post- hurricane data can be collected, and flooding extent can be determined using the method created in Phase 1
- Produce and Document output that can be ingested by ArcGIS.

## Project Phases

### 1. Use NDVI to determine if flooding has occured within an example DemoZone.
Phase 1 Tasks
- Volunteers will register with trial accounts with Sential and set up their Dev Environment 
- DAs will Provide Data and Locations Information and be available for Questions
- Provide Example Notebook of commonly used sentinel-hub bindings 
- Provide the location of the DemoZone.
- Provide Brief on Tidal Data
- Team will work on creating code that determines if flooding has occurred within the DemoZone 
Phase 1 Deliverables
- Volunteers will produce a proof of concept that flooding can be determined via NDVI and Sentinel for a DemoZone. 
- Volunteers will produce an algorithm for incorporating tidal data into flooding analysis.

## Phase 1 Assumptions (A) & Questions (Q)
The DemoZone is a small pre-determine subset of the full AOI that will be used to build DataKind volunteer capacity.  The DemoZone, Example Notebook, and tidal data brief will be produced by the DAs prior to DataDive.

## OPEN QUESTIONS
1. Confirm Projection between Json, and Shapefiles is the same.  
2. Build Large Bounding Boxes for areas in the demo zone 
    2a. Define ‘Large’ in pixes for satelitte data 
3. Define what ‘Flooding’ means for an area using NDVI 
4. Investigate how the tidal data can be used with the areas of interest to not over estimate flooding

## Quick Start 
Optional:If you need a 5 minute crash course of GIS and Satelitte Data Review this deck: https://drive.google.com/open?id=1md32EbjZgsf0u4t-C06H65s-u_IGKUq4KpOExdwCNk4
1. Clone the repository and Navigate to the Examples Folder. 
2. Follow the Examples to working with eo-learn and Sentinel

### 2. Design and Implement a near-real time utilization of the phase 1 algorithm
Phase 2 Tasks
Volunteers Design and Implement a system where pre-hurricane data can be collected, post- hurricane data can be collected, and flooding extent can be determined using the method created in Phase 1 for the AOI
Volunteers will conceive an efficient way to store data used for analysis 
Volunteers will design and Implement a workflow that would Trigger Phase 2 when there is an impending hurricane/recent.
Phase 2 Deliverables
Volunteers will produce a python code that is capable of producing a ArcGIS map of beaches and Marshes in the AOI that were recently flooded. 
Phase 2 Assumptions (A) & Questions (Q)
DAs will provide a specialized example Python Notebook containing common Sential Bindings and processes in order to alleviate the learning curve for volunteers. 

### 3. Documentation and Bundle Deliverables
Phase 3 Tasks
Create slide deck and narrative for Sharing with DataKind and Project Partners, the Audubon Society 
Create Well documented Python Notebooks and ReadMes to share with Project Partners
Pick a Location for HH 
Phase 3 Deliverables
Deck of the Process to Share with Project Partners 
CodeBase to share with Project Partners 
Phase 3 Assumptions & Open Questions

## References
Summary of Original Proof of Concept 
https://drive.google.com/open?id=1fehFrLv5ccBBuqWtm754PrOjobXQZkx1SWieTiV6haY

