## Welcome!

This is the README file for my Lab 2 project with information about the project including my reflective analysis.

**Here is the link to my map:** https://isabellamontecalvo.github.io/isabellamontecalvo-web/lab2/index4.html

Here is the [raw data](https://data.torontopolice.on.ca/datasets/TorontoPS::bicycle-thefts-open-data/about) for my bike theft data provided by Toronto Police Service Public Safety Data Portal. **NOTE:** This data was updated on March 28, 2023, after I had started downloading and using the data, thus it may differ slightly. Regardless, the GEOJSON data I used is uploaded to this folder.

You can see a screenshot of my map here where the pointer is showing a 7.5 magnitude earthquake:
![alt text]()


###Reflective Analysis

I designed this map specifically for bike users and/or prospective bike users in the Toronto area. Through this map, I hoped to enlighten bike users on the history of bike thefts in the Toronto area so that they would be aware and cautious of:
1. Where they lock their bikes up
2. What times they’re locking their bikes up
3. How the cost of a bike influences thefts
4. How thefts have varied over the years

These insights are all aimed at increasing public safety and awareness in regard to bikes. Using these filters in combination will hopefully allow for comparison and a greater understanding of the threat of bike theft. Thus bike users will be more informed about the safest place, time, type of bike and year when locking up their own bikes.

Ultimately, the map aims to answer the question: if my bike costs X and I live here (Y) and I usually lock it up around Y or Z at this time (W), how likely is it to get stolen? And does this change from year to year?

Prospective bike users might also benefit from this map, as they might be looking to purchase a bike but are concerned about bike theft before buying. Using this map may give them a clearer picture of the risks they run in terms of buying certain type of bike and where and when they are likely to lock it up.

The map uses a simple, light grey basemap in order to limit the number of colours, preserve visual harmony and highlight the points and the colour of those points. Against a plain background, the bike theft points stand out clearly in contrast. The map shows bike thefts from 2018-2022 -  I included the most recent years so that data would be most up-to-date and users can compare bike thefts across the years (using the toggle function). At the same time, users can change the time at which the theft occurred, thus comparing theft times across years (seeing how it’s changed). It seems as though bikes are consistently stolen around Yonge street, regardless of year or cost of bike, though it does vary depending on time (most thefts there are during the day). Particularly interesting is the 2020 pandemic year, which shows higher thefts during the day eg. 1pm (very interesting as people might’ve had more opportunities to steal during the day). My data also included the cost of the bike that was stolen. I wanted to represent that in order to show bike users what types of bikes (eg. expensive or cheap) are targeted using a colour hierarchy, where they are targeted and how that changes depending on the time of day (slider). I tried to adjust the circle’s symbolisation (radius) based on the cost of the bike, though this didn’t offer any helpful insights. Users also have the ability to mouse over a point to show the cost of the bike in CAD for further analysis.
### Critiques
The map does well to show earthquake activity at a low zoom level, but becomes admittedly less helpful at a higher zoom level (larger scale). The heat map gets a bit too cluttered/congested at larger zoom levels, though you can still see the individual heat map points. A way that this map would be greatly improved would by switching to circles at a higher zoom level (a conceptual generalisation technique). As the user zooms into the heatmap, the points stop overlapping visually and it is no longer necessary to show their distribution and density. At this point, it would have been better to show the points themselves and allow viewers to explore the data interactively. I could have done this, though I was a bit short on time and it was difficult, so I didn’t manage to, but the general principle is outlined here: https://docs.mapbox.com/help/tutorials/make-a-heatmap-with-mapbox-gl-js/. I am also a bit disappointed that despite adjusting the properties of my heatmap, distinguishing the differences between magnitude points is very poor, eg. the difference between a 7.5 and 4.4 magnitude earthquake is minor on my heat map. Again, this could be improved by using circles as mentioned above. Unfortunately I did not have the time to do a peer-critique.

### Resources
A list of resources that I am indebted to!
* https://docs.mapbox.com/help/tutorials/studio-heatmap-tutorial/
* https://docs.mapbox.com/mapbox-gl-js/example/heatmap-layer/
* https://docs.mapbox.com/help/tutorials/make-a-heatmap-with-mapbox-gl-js/
* https://docs.mapbox.com/mapbox-gl-js/style-spec/layers/#layout-heatmap-visibility
* https://github.com/UBC-GEOB472-Spring2020/tracyw04-web/tree/master/lab1
