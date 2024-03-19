# Final Project Proposal

## Members

Eric Chong, Daniel Dong, Jo Nguyen

## Research question:  

> How does the accessibility of green spaces through the public transit system influence urban sustainability and environmental justice in Vancouver? 

## Intellectual justification:  

The intellectual motivation behind this project focuses on addressing the intersecting challenges of urban accessibility and environmental justice within Vancouver. By creating an accessibility map that helps to illustrate TransLink bus routes onto green spaces, we aim to highlight areas with inadequate access to nature, particularly amongst marginalized communities. Building upon established basic urban planning principles and web cartography methodologies learnt in GEOS 472, this initiative works as a call to action with insights that can be utilized towards future development plans and for planners to reference when looking to strategically implement green space based on spatial distribution - fostering a more inclusive and sustainable urban environment. Ultimately, this project represents a vital step towards fostering equitable accessibility to green spaces.

## Tentative data sources:  

- [Real-time Transit Information (RTTI)-Translink API](https://www.translink.ca/about-us/doing-business-with-translink/app-developer-resources/rtti)

- [LiDAR 2022](https://opendata.vancouver.ca/explore/dataset/lidar-2022/information/)

- [Greenways](https://opendata.vancouver.ca/explore/dataset/greenways/information/?location=14,49.25169,-123.13447)

- [Parks](https://opendata.vancouver.ca/explore/dataset/parks-polygon-representation/map/?location=13,49.2524,-123.11717)

- [Non-Market Housing](https://opendata.vancouver.ca/explore/dataset/non-market-housing/map/?location=14,49.25613,-123.11747)

## Potential maps and geographical visualizations:  

### We are planning on producing the following layers:

-  Vancouver's 3D representation using LiDAR data.
	- Similar to this [example](https://github.com/potree/potree).
-  Vancouver's park space.
-  Vancouver's greenways.
-  Vancouver's non-market housing (subsidized housing).
-  Vancouver's bus stops, routes, and live bus information.
-  Vancouver's 3D terrain. 

### And interactivity: 

- Scale bar and navigation control panel.
- A menu/sidebar with buttons that can toggle layers on/off.
	- The button for loading the LiDAR files is only clickable on larger zoom levels, so that a controlled number of files would be loaded at a time, avoiding using too much memory. 
- The ability for map users to click anywhere on the map and being automatically shown the cloest transit route to the nearest park 
- The ability to estimate travel time via transit based on live traffic.
- The ability to show all related live bus location and routes when hovering over a bus stop.

## Coding:  

We will be utilising [Mapbox Studio](https://www.mapbox.com/mapbox-studio), [Mapbox GL JS](https://docs.mapbox.com/mapbox-gl-js/guides/), [Potree](https://github.com/potree/potree), and potentially [Deck.gl](https://deck.gl/) and/or [Cesium JS](https://cesium.com/platform/cesiumjs/).

- On the topic of loading the LiDAR files, we might pick between one of the following approaches in order to appropriately display the correct files:
	1. Download all 181 LAS files (and potentially converting them all into LAZ format), then use Potree to load the files. 
	2. Download all 181 LAS files and convert them all into 3D tiles, and use Cesium/Deck.gl to load them.
	3. Via one of the fields of the 2022 LiDAR geojson file, retrieve the link to the ZIP files that contains the LAS files, unzip them and use Potree to load them. 
	4. Or maybe host all files on an online tile server...
- We intend to use Translink's API to query all information related to Vancouver's transit system (i.e. live bus locations, coordinates for bus stops and routes, etc.). 

## Cooperation: 
- We have already created a new public GitHub repository for our final project to help with file/data management. 
- We are using Discord as our mean of communication.
- We seek to find the most feasible way to involve every member in each stage of the project. The division of labor will be reflected upon and assessed again accordingly at the end of the project to correctly evaluate contribution. While maintaining flexibility, we ensure equitable involvement and ensure both efficiency and effectiveness.
