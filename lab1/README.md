## Welcome!

This is the README file for my lab 1 project with information about the project including my reflective analysis.

**Here is the link to my map:** https://isabellamontecalvo.github.io/isabellamontecalvo-web/lab1/earthquakes.html

Here is the [raw data](https://earthquake.usgs.gov/fdsnws/event/1/query.geojson?starttime=2023-02-02%2000:00:00&endtime=2023-03-04%2023:59:59&minmagnitude=2.5&eventtype=earthquake&orderby=time) from my query for earthquake data provided by USGS.

You can see a screenshot of my map here where the pointer is showing a 7.5 magnitude earthquake:
![alt text](https://isabellamontecalvo.github.io/isabellamontecalvo-web/lab1/Earthquake_7.5mag.png)


### Data Choice
On February 6, 2023, a powerful moment magnitude earthquake of 7.8 struck southern and central Turkey and northern and Western Syria. A series of strong tremors and aftershocks devastated the area, causing widespread damage and tens of thousands of fatalities. Two weeks later on February 20, 2023, an additional 6.3 magnitude earthquake hit southern Turkey, causing additional deaths and injuries ([World Vision, 2023](https://www.worldvision.org/disaster-relief-news-stories/2023-turkey-and-syria-earthquake-faqs)).

In the last month, the world’s efforts have been directed towards aiding Turkey and Syria in search and rescue teams, recovery efforts, and providing relief supplies. Hearing about this, I chose to map earthquake activity in the region, and thus the initial focus of my map is centred on coordinates around Turkey and Syria. The purpose of the map is to show relief organizations working to deliver relief supplies the activity of earthquakes in the region, including where they are occurring when they occurred and their magnitude. As there was a subsequent earthquake on February 20th, I thought it would be useful for these relief organisations to know of any further possible earthquakes so that they can prepare accordingly/take precautions. As these relief organisation often carry supplies via trucks and therefore roads, I included the road layer in my map. My aim was to make a heat map of the earthquake activity in the region, with the ability to mouse over the earthquakes to find out the date, location and magnitude of the earthquake for more detailed analysis. 

### Styling

The basemap was chosen from the Mabox Street template (to prioritise accurate and legible styling of road and transit networks), with a simple, neutral grey for land and blue for water vector background. I wanted to minimise the number of colours used in the background to preserve visual harmony, contrast the main elements (land and water) and highlight the heat map. I kept the contextual layers of country boundaries (but removed state/province/county boundaries as it was unnecessary for the purposes of this map), names of countries and cities (to show what cities are affected and/or if they can be reached), and simple hill shading (to show terrain) and waterbodies. Country and city names were kept in black with a white halo to preserve their legibility. Natural feature icons were kept but only shown at a higher zoom level for further detail. The road network component was important for navigation for relief vehicles, so I picked the “navigation” setting for the road network to emphasise the main roads in orange/yellow lines. I kept the labels of the main roads but changed the icons of those labels to be monochrome to lower them on the visual hierarchy scale and not detract from the heat map. The colour hierarchy defaults of the roads were kept, showing thicker orange main motorways at a lower zoom level.

The heat map was chosen to represent my data to visualise point density and relative differences between points based on the earthquake data property magnitude. All were chosen to change based on zoom range and data range. Within the heat map layer, using the paint property, I was able to manipulate my heat map. I chose colours based on Colour Brewer’s selection for heat (darker reds indicating higher density, thus using emotion to engage understanding - the connotation of red implies urgency) and changed the rate of change for density to increase by 0.2 for each class to emphasise difference between classes. Heat map weight was chosen to be an exponential rate of change, from the lowest magnitude 2.5 at a weight of 1 and the highest (7.8) at a weight of 2, heat map radius was chosen to be 10px at Zoom 0 and 40px at zoom 22 (increasing the pixel value made the heat map smoother but less detailed at a higher zoom), and finally the heat map opacity was chosen at 0.75 to try and emphasise the heat map itself while also allowing users to see the roads and place names below it.

### Critiques
The map does well to show earthquake activity at a low zoom level, but becomes admittedly less helpful at a higher zoom level (larger scale). The heat map gets a bit too cluttered/congested at larger zoom levels, though you can still see the individual heat map points. A way that this map would be greatly improved would by switching to circles at a higher zoom level (a conceptual generalisation technique). As the user zooms into the heatmap, the points stop overlapping visually and it is no longer necessary to show their distribution and density. At this point, it would have been better to show the points themselves and allow viewers to explore the data interactively. I could have done this, though I was a bit short on time and it was difficult, so I didn’t manage to, but the general principle is outlined here: https://docs.mapbox.com/help/tutorials/make-a-heatmap-with-mapbox-gl-js/. I am also a bit disappointed that despite adjusting the properties of my heatmap, distinguishing the differences between magnitude points is very poor, eg. the difference between a 7.5 and 4.4 magnitude earthquake is minor on my heat map. Again, this could be improved by using circles as mentioned above. Unfortunately I did not have the time to do a peer-critique.

### Resources
A list of resources that I am indebted to!
* https://docs.mapbox.com/help/tutorials/studio-heatmap-tutorial/
* https://docs.mapbox.com/mapbox-gl-js/example/heatmap-layer/
* https://docs.mapbox.com/help/tutorials/make-a-heatmap-with-mapbox-gl-js/
* https://docs.mapbox.com/mapbox-gl-js/style-spec/layers/#layout-heatmap-visibility
* https://github.com/UBC-GEOB472-Spring2020/tracyw04-web/tree/master/lab1
