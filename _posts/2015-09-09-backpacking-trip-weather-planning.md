---
layout:     post
title:      Backpacking trip weather planning
date:       2015-09-09 
summary:    Don't let the weather surprise you
categories: backpacking weather emigrant_wilderness
---

It is surprisingly easy to freeze your ass off in the High Sierras. Luckily, our group avoided being caught unprepared by a cold front camping this past weekend at Y Meadow Lake in the Emigrant Wilderness. I'm quite sure that if we hadn't done the following backpacking trip weather planning we would have had to cut the trip short. Here are the most useful insights:

##Finding the right weather station

Not all weather stations are created equally. A forecast is offerred for only the most popular/reliable weather stations. Example: while the Gianelli meadow weather station, GNLC1, is the closest weather station to Y Meadow Lake, no one uses it to create a weather forecast. 

The next closest weather station is [Pinecrest lake](http://www.wunderground.com/weather-forecast/zmw:95364.1.99999) which does provide a temperature forecast. The recorded low temperature on the first night of our trip as reported from Pinecrest Lake was around 52 ˚F. This recorded data matched closely with the forecast at the time <a id="00" href="#01">[0]</a>. If we had looked no further we would have been in serious trouble. 

{% include image.html url="/images/backpacking-trip-weather-planning-station.jpg" description="Pincrest Lake, Y Meadow Lake, and the closest weather stations." %}

##Account for change in elevation

Pinecrest lake is poor indicator of expected temperature because its elevation is only 5600 feet, a full 3200 feet below our campsite. So while the overall proximity is close enough to believe the precipation forecast, the temperature forecast won't reflect the [dry adiabatic lapse rate](https://en.wikipedia.org/wiki/Lapse_rate#Dry_adiabatic_lapse_rate). Basically, for dry areas (like the High Sierras), there is a temperature decrease of roughly 5.5 ˚F for every 1000 ft gain in elevation. That balmy nighttime low of 52 ˚F at Pinecrest is not even in the same league as the frigid 35.5 ˚F at Y Meadow. 

{% include image.html url="/images/backpacking-trip-weather-planning-wunderground.jpg" description="52 ˚F nighttime low at - 16.5 degrees of dry adiabatic lapse = 35.5 ˚F expected low" %}

##Account for change in terrain

There aren't any numbers I can reference here, but here's some very general tidbits I've encountered over the years:

* Take a look at the topographic map for the area to get an idea of where the wind will be coming from. 

* Camping in an exposed area means there's likely to be a near-constant breeze (e.g. near a lake, above the tree line, an open field, beach, etc.). Wooded areas tend to break up the wind and reduce the effect of [wind chill](https://en.wikipedia.org/wiki/Wind_chill). In the case of our trip, we had a constant breeze during the day that died down at night. 

##What we changed

Since we were initially planning on the temperature not dropping below ~50 ˚F, we did the following to prepare for an estimated 35 ˚F trip:

* Upgraded the sleeping bags to properly rated mummy bags (thanks Will and Kim!)
* Everyone brought their own ultra-warm hat, gloves, and wool socks (for sleeping)
* Double check that we had foolproof methods of boiling water and building campfires

##How we fared

We departed from Gianelli trailhead at 1:00pm 9/5 and returned at 11:30am 9/7. Since [GNLC1](http://weather.gladstonefamily.net/site/GNLC1) reports historical data, I was able to do a quick import of an XML feed into Google Sheets and attach some fudge-factor error bars. As you can see, the Pinecrest temperature forecast combined with dry adiabatic lapse was a great proxy for what we encountered <a id="01" href="#11">[1]</a>. I'd be lying if I said we were toasty warm both nights, but we were all able to at least make it through the night. Not a smashing success, but overall we had a wonderful trip and didn't let the cold get the best of us. 

<iframe style="width:600px; height:370px; display: block; margin-left: auto; margin-right: auto" src="https://docs.google.com/spreadsheets/d/1gqB1HuNTizQlu8ioeg1sK1vmAPiAskvv_XlFTggFbbM/pubchart?oid=1664143097&amp;format=interactive"></iframe>

##Other resources used for researching this post

* Apparently the [California Bureau of Reclamation](http://cdec.water.ca.gov/cgi-progs/queryF?s=GNL&d=07-Sep-2015+11:10&span=51hours) maintains the GNLC1 weather station. 
* MesoWest does some kind of quality control analysis on weather station reporting. [You can see here that GNLC1 has been acting up recently](http://fam.nwcg.gov/roman/cgi-bin/meso_base_past.cgi?stn=GNLC1&unit=0&time=LOCAL&day1=5&month1=09&year1=2015&hour1=0). I may make a point to reference this data next time I'm doing some backpacking trip weather planning. 
* The [NOAA Hydrometeorological Automated Data System (HADS)](http://www.nws.noaa.gov/oh/hads/) also maintains a large number of weather stations. GNLC1 is included and you can search for it via the NWSLI ID search box.   


<a id="01" href="#00">[0]</a> I'd show the original forecast, but I didn't take a screenshot so I have to use historical data.

<a id="01" href="#11">[1]</a> In case anyone's keeping track, GNLC1 at Gianelli Meadow is located at an elevation of 8640 feet, Y Meadow Lake is 8750 feet, and Pinecrest Lake is 5640 feet. 
