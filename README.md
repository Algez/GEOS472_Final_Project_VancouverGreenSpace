## Members
Eric Chong, Daniel Dong, Jo Nguyen

## Intellectual justification:  

The intellectual motivation behind this project focuses on addressing the intersecting challenges of urban accessibility and environmental justice within Vancouver. By creating an accessibility map that helps to illustrate TransLink bus routes onto green spaces, we aim to highlight areas with inadequate access to nature, particularly amongst marginalized communities. Building upon established basic urban planning principles and web cartography methodologies learnt in GEOS 472, this initiative works as a call to action with insights that can be utilized towards future development plans and for planners to reference when looking to strategically implement green space based on spatial distribution - fostering a more inclusive and sustainable urban environment. Ultimately, this project represents a vital step towards fostering equitable accessibility to green spaces.

## Research question(s):  
A clear statement of the question(s) you hope to address (or pose for the reader) in some fashion.

## Data Sources (Tentative):  

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
-  Vancouver's non-market housing.
-  Vancouver's bus stops, routes, and live bus information.
-  Vancouver's 3D terrain. 

### And interactivity: 
- Scale bar and navigation control panel.
- A menu/sidebar with buttons that can toggle layers on/off.
	- The button for loading the LiDAR files is only clickable on larger zoom levels, so that a controlled number of files would be loaded at a time, avoiding using too much memory. 
- The ability for map users to click anywhere on the map and the automatically shows the cloest route to the nearest park.
- 

## Coding:  
Reflect on how and why you plan to make good and relevant use of coding. Are there new features or libraries you might want to try out?

- We will be utilising Mapbox Studio, Mapbox GL JS, Potree, and potentially deck.gl and/or Cesium JS.
- On the topic of loading the LiDAR files, we might download and convert all the LAS files
- Potentially we can

**Questions:  Focused questions you have for me and/or for yourselves moving forward!**

## Cooperation: 
- We have already created a new public GitHub repository for our final project, so that all of our contributions can be visualized.
- We are using Discord as our way of communication.
-  


It is crucial that you think about and offer us a plan for how the group will work together. Consider articulating an initial division of labour (mixed with cooperation, I do hope!) among the group that is equitable. Such a plan should detail how  _**each**_  group member will demonstrate how they have learned the material of the course and can apply it. We will be reflecting back on these statements as your work moves forward. 
