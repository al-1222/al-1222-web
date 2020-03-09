# Lab 2 - High Speed Internet Cafes in Beijing Within Walking Distance 


<strong>Link: https://editor.p5js.org/angela_22/full/DXB_pHcH </strong>

<i>Click on <strong>LAB2</strong> in top left corner to open edit mode to see entire commented code.</i>

Screenshot:
![alt text](https://github.com/UBC-GEOB472-Spring2020/al-1222_Lab2/blob/master/Lab2Screenshot.PNG "Logo Title Text 1")

<strong>Collaboration and reliance on other sources: </strong>

I drew the base maps from Leaflet Tilelayer Provider Demos, and slightly modified a GeoJSON file on Beijing Cafes from a Github Repository: https://github.com/ElaWorkshop/awesome-cn-cafe/blob/master/beijing.geojson. I also drew piece of code from class demos provided on slides, and other pieces of code from other online users, which are commented in the code itself (above link). 

<i>Peer map critique:</i> Lucas Vianna noted that it would be beneficial to add a descriptor about the radius of the orange buffer circle, and Ema Zizic suggested that having the Light version of the basemap as the first selection rather than the transport map would be a better visual choice. I was able to implement both suggestions. I reviewed Lucas Vianna's code and suggested buffers around the points may be a good idea to indicate how many ski resorts are within a certain distance of an airport using Turf.js. 

<strong>Reflective Analysis</strong>

This map is designed using Leaflet for fast-paced working or studying citizens of Beijing, and the question I wanted this map to answer was what is the nearest cafe within a maximum 20 minute walk with the highest internet speed. I believe my map was able to accomplish this, but only to a certain extent. My map incorporates interactivity with a selectable point symbol that users can assert a choice in where they want to place their "starting point". It then creates selections using buffer filter on points within this circle and these selected points have a pop-up option indicating name as well as internet speed. Layer control is also implemented for individuals to view a basemap that allows for more transportation planning in comparison to a cleaner basemap for location selection. An understanding of arrays through the readings as well as through class was particularly helpful for learning to store selected points in an array before removing them at new selection. 

<i>Limitations:</i>
During the creation of this map, I have repeatedly attempted to alter the symbology and use mouse hover instead of click open, and unfortunately I was unsuccessful. I wanted to change the symbology in accordance to the internet speed; however, despite multiple attempts of either calling on icon urls from Github or installing icon packages (https://github.com/sigma-geosistemas/Leaflet.awesome-markers), the map only showed a missing PNG icon. 
![alt text](https://github.com/UBC-GEOB472-Spring2020/al-1222_Lab2/blob/master/Missingpngicon.PNG "Logo Title Text 1") I had also wanted to add other GeoJSON layers to my layer control element, and I did create my own GeoJSON file of universities in Beijing, and use Turf.js to create buffers. I think this is definitely doable and I will likely work on this code more in my own time, but I unfortunately did not have the time to operationalize this for this submission. 

I also had really wanted to have a slider option to change the radius of the circle, and I attempted to use the Turf.js code demonstrated in class on Tissot circles; however, I was unable to modify it to become compatible with my existing code. It would also be helpful to have a table beneath or beside the map to show other feature properties of the points in selection, such as the reviews, which was a property included in the GeoJSON. I had originally wanted to use a search filter mechanism from an example on Mapbox, and while I was successful, I found that it would, in reality, not be a very useful interactive element as users can search up cafe names through other means (eg. Baidu Maps). Nonetheless, I think a search filter could've been beneficial if the query was for roads, for districts, instead of cafe names. 
