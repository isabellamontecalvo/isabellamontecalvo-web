## Welcome!

This is the README file for my Lab 2 project with information about the project including my reflective analysis.

**Here is the link to my map:** https://isabellamontecalvo.github.io/isabellamontecalvo-web/lab2/index4.html

Here is the [raw data](https://data.torontopolice.on.ca/datasets/TorontoPS::bicycle-thefts-open-data/about) for my bike theft data provided by Toronto Police Service Public Safety Data Portal. **NOTE:** This data was updated on March 28, 2023, after I had started downloading and using the data, thus it may differ slightly. Regardless, the GEOJSON data I used is uploaded to this folder.

You can see a screenshot of my map here where the pointer is showing a 7.5 magnitude earthquake:
![alt text](https://isabellamontecalvo.github.io/isabellamontecalvo-web/lab2/Biketheftmap.png)


### Reflective Analysis

I designed this map specifically for bike users and/or prospective bike users in the Toronto area. Through this map, I hoped to enlighten bike users on the history of bike thefts in the Toronto area so that they would be aware and cautious of:
1. *Where* they lock their bikes up
2. What *times* they’re locking their bikes up
3. How the *cost of a bike* influences thefts
4. How thefts have varied over the years

These insights are all aimed at increasing public safety and awareness in regard to bikes. Using these filters in combination will hopefully allow for comparison and a greater understanding of the threat of bike theft. Thus bike users will be more informed about the safest place, time, type of bike and year when locking up their own bikes.

Ultimately, the map aims to answer the question: if my bike costs X and I live here (Y) and I usually lock it up around Y or Z at this time (W), how likely is it to get stolen? And does this change from year to year?

Prospective bike users might also benefit from this map, as they might be looking to purchase a bike but are concerned about bike theft before buying. Using this map may give them a clearer picture of the risks they run in terms of buying certain type of bike and where and when they are likely to lock it up.

The map uses a simple, light grey basemap in order to limit the number of colours, preserve visual harmony and highlight the points and the colour of those points. Against a plain background, the bike theft points stand out clearly in contrast. The map shows bike thefts from 2018-2022 -  I included the most recent years so that data would be most up-to-date and users can compare bike thefts across the years (using the toggle function). At the same time, users can change the time at which the theft occurred, thus comparing theft times across years (seeing how it’s changed). It seems as though bikes are consistently stolen around Yonge street, regardless of year or cost of bike, though it does vary depending on time (most thefts there are during the day). Particularly interesting is the 2020 pandemic year, which shows higher thefts during the day eg. 1pm (very interesting as people might’ve had more opportunities to steal during the day). My data also included the cost of the bike that was stolen. I wanted to represent that in order to show bike users what types of bikes (eg. expensive or cheap) are targeted using a colour hierarchy, where they are targeted and how that changes depending on the time of day (slider). I tried to adjust the circle’s symbolisation (radius) based on the cost of the bike, though this didn’t offer any helpful insights. Users also have the ability to mouse over a point to show the cost of the bike in CAD for further analysis.

### Critiques
I’m not sure how helpful the cost of bike coloration is - perhaps there is not enough difference between the colours to be useful. As I mentioned earlier, I tried to adjust the radius of the circle points based on the cost of the bike for further differentiation, but again, I’m not sure that I had enough classes to properly distinguish between price levels using size. To amend this, I added the mouseover function to show the exact cost of a bike. Unfortunately, my skill with CSS is a bit rough, so the location of the Cost of bike legend is a bit janky. I also attempted to show ‘all’ the bike thefts for all the years, but I don’t think my code worked.

I’m wondering if adding another toggle option for differentiating between residential, commercial and other areas would have been helpful. Adding the day of the week that bikes were stolen could add a useful dimension as well.

### Resources
A list of resources that I am indebted to!
* https://docs.mapbox.com/help/tutorials/show-changes-over-time/
* https://docs.mapbox.com/help/tutorials/choropleth-studio-gl-pt-2/
