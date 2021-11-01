### Filling in the Gaps: Mapping Potholes in Oakland

**Research Question**

For our project, we're looking at **what parts of Oakland are most affected by road deterioration and is the city’s repaving program adequately addressing those areas?**

This overarching question will involve us addressing several other questions including: 

- How are 311 road service request distributed throughout Oakland?
- What are the demographics of areas with higher or lower numbers of requests? 
- Are 311 road complaints addressed faster in certain parts of the city?
- What are the demographics of those areas that recieve faster or slower response times? 
- How have the trends in any of the prior questions changed over time? 
- How does the City's repaving work align with 311 requests or demographic data? 

**Why is this important?**

While at first road condition doesn't seem like the most pressing challenge facing society, roads are a major infrastructural resource and reflection of government involvement in an area. People interact with them daily, and a poorly maintained road can damage bikes, cars, buses, and other transport vehicles. Aside from the purely tangible repercussions of street deterioration, a badly damaged road can show local government's negligence or indifference toward specific areas. Often, communities of color and low-income communities are most likely to face government indifference, so we are seeking to find whether that is the case when it comes to Oakland's paving procedure, as well as how government response has changed over time in different neighborhoods. While mapping this data will not inherently solve discriminatory practices, it may provide insight on other issues of government negligence or encourage change.

**Spatial and Time Scope**

City of Oakland, 2009 to Present day (Oct 2021). 

Specifcally we're looking at requests made in 2009 and then in 2019 for comparison, although many of these 311 requests are still being addressed so that is why the scope runs to present day. 

**Roles**

- Income Master Mary: Mapping census income data, 311 pothole requests and time til request closure for 2009.
- Oakland Oracle Nick: Mapping census race data, 311 pothole requests and time til request closure for 2019.

**Data Sources**

Original Mapping:
- [Oakland 311 Complaint Data](https://data.oaklandca.gov/Infrastructure/Service-requests-received-by-the-Oakland-Call-Cent/quth-gb8e)
    * This file contains all data of Oakland's 311 complaint reporting system from 2009 to the present, which we will filter to include just road complaints for visualization purposes. Our group does have concerns about potential bias in which demographics may use 311 more often, so in the second half of the course we will try to account for this by normalizing the road specific 311 requests with all 311 requests. This might tell us if there's parts of the city submitting more road related 311 requests than we would expect. 
- 2019 ACS Census Data for [income](Group Assignments/Data/ACSST5Y2019.S2001_2021-10-10T213455.zip) and [race](Group Assignments/Data/2010_Pop_Tract_County.xls)
   * We are including census data for the city to visualize the Oakland's demographics by race and income, and eventually update our current cenuss tract analysis to a census blck group level analysis. We will use this information to see whether 311 complaints or the speed to which the city responds to reported issue may be influenced by demographics of an area.
- [Alameda County Census Block Groups](Group Assignments/Data/Alameda_Census_Blocks_2010.geojson) 
   * Given the large amount of data points with this analysis, we will use census block polygons to group our points to improve visibility. We couldn't find Oakland specific census block geodata, but this shouldn't be an issue since we're just matching points in Oakland. There is a concern that while census blocks are roughly normalized for population, they are not standardized in size. Thus there could be a disparity in the amount of roads located in blocks, thereby leading to more requests. The team has discussed this issue with a TA and it seems accounting for this would prove challenging, so this is just apotential issue to be aware of in our analyses. 

Existing Map Data Used for Comparison:
- [Measure KK funding](https://oakgis.maps.arcgis.com/apps/webappviewer/index.html?id=dbd0e3cbe71b4fa1abbaa33ab1b00deb)
- [Oakland Road Condition Funding](https://oakgis.maps.arcgis.com/apps/webappviewer/index.html?id=d56c2b6ae597493b813be96015ae73b3)
   * We plan to use this data as part of the same structure, with the first set showing repaving completed before the 3-year repavement plan was implemented in 2019. The second dataset shows repaving that has been completed and is planned for the future under the 3-year repavement plan.

**Visual Flow Chart**

 <img src="https://github.com/maryalicewilliams/Nick_MaryAlice_Potholes/blob/main/Group%20Assignments/Images/Data%20Flow%20Chart.jpeg" width="700">


**Conclusion (so far)**

Thus far our maps have been a little crowded or without obvious visible trends. Overall we know the city's median response time to 311 road service requests dropped from 51 to 32 days from 2009 to 2019, so that was interesting. I think as part of our next step we want to explore that change a little bit more in identifying if that change was equal across the map or if it was more concentrated in certain communities. 

Specifically, in the second half of the class we hope to: 

- Map our census data to census block groups. 
- Identify the demographic characteristics of census blocks outliers.
- Start the analysis from a demographic characteristics. Map median closure time for census blocks (examples):
      - Where 30% or more of the population is black or white
      - That are in the bottom ¼ or top ¼ in median income 
- Normalize 311 road requests with overall 311 request rate. 
- Incorporate the City's paving data. 

