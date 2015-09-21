---
layout:     post
title:      Backpacking trip weather planning
update_date:       2015-09-14 
summary:    Don't let the weather surprise you
tags: 
  - backpacking 
  - weather 
  - emigrant wilderness
allow_comments: TRUE
---

It is surprisingly easy to freeze your ass off in the High Sierras. Luckily, our group avoided being caught unprepared by a cold front while hammock camping this past weekend at Y Meadow Lake in the Emigrant Wilderness. I'm quite sure that if we hadn't done the following backpacking trip weather planning we would have had to cut the trip short. Here are the most useful insights:

##Current top weather services

[Lifehacker](http://lifehacker.com/5897973/five-best-weather-web-sites) polled their followers and put together the following list (in order or popularity):

1. [Weather Underground](http://www.wunderground.com/) (aka, Wunderground)
2. [National Weather Service](http://www.weather.gov/) - not to be confused with weather.com. 
3. [Forecast.io](http://forecast.io/)
4. [Weather Spark](https://weatherspark.com/)
5. [The Fucking Weather](http://thefuckingweather.com/)

While all of these services are perfectly fine for precipitation and large-scale weather patterns, for the Emigrant Wilderness I care most about temperature. For that I want to get get a lot more specific. 

##Finding the right weather station

Not all weather stations are created equally. A forecast is offered for only the most popular/reliable weather stations. Example: while the Gianelli meadow weather station, [GNLC1](http://weather.gladstonefamily.net/site/GNLC1), is the closest weather station to Y Meadow Lake, no one uses it to create a weather forecast. 

The next closest weather station is [Pinecrest lake](http://www.wunderground.com/weather-forecast/zmw:95364.1.99999) which does provide a temperature forecast. The recorded low temperature on the first night of our trip as reported from Pinecrest Lake was around 52 ˚F. This recorded data matched closely with the forecast at the time <a id="01" href="#10">[0]</a>. If we had looked no further we would have been in serious trouble. 

{% include image.html url="/images/backpacking-trip-weather-planning-station.jpg" description="Pincrest Lake, Y Meadow Lake, and the closest weather stations." %}

##Account for change in elevation

Pinecrest lake is poor indicator of expected temperature because its elevation is only 5600 feet, a full 3200 feet below our campsite. So while the overall proximity is close enough to believe the precipitation forecast, the temperature forecast won't reflect the [dry adiabatic lapse rate](https://en.wikipedia.org/wiki/Lapse_rate#Dry_adiabatic_lapse_rate). Basically, for dry areas (like the High Sierras), there is a temperature decrease of roughly 5.5 ˚F for every 1000 ft gain in elevation. That balmy nighttime low of 52 ˚F at Pinecrest is not even in the same league as the frigid 35.5 ˚F at Y Meadow. 

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

We departed from Gianelli trailhead at 1:00pm 9/5 and returned at 11:30am 9/7. Since [GNLC1](http://weather.gladstonefamily.net/site/GNLC1) reports historical data, I was able to do a quick import of an XML feed into Google Sheets and attach some fudge-factor error bars. As you can see, the Pinecrest temperature forecast combined with dry adiabatic lapse was a great proxy for what we encountered <a id="02" href="#20">[1]</a>. I'd be lying if I said we were toasty warm both nights, but we were all able to at least make it through the night. Not a smashing success, but overall we had a wonderful trip and didn't let the cold get the best of us. 

<iframe style="width:600px; height:370px; display: block; margin-left: auto; margin-right: auto" src="https://docs.google.com/spreadsheets/d/1gqB1HuNTizQlu8ioeg1sK1vmAPiAskvv_XlFTggFbbM/pubchart?oid=1664143097&amp;format=interactive"></iframe>

##Other resources used for researching this post

* Apparently the [California Bureau of Reclamation](http://cdec.water.ca.gov/cgi-progs/queryF?s=GNL&d=07-Sep-2015+11:10&span=51hours) maintains the GNLC1 weather station. 
* MesoWest does some kind of quality control analysis on weather station reporting. [You can see here that GNLC1 has been acting up recently](http://fam.nwcg.gov/roman/cgi-bin/meso_base_past.cgi?stn=GNLC1&unit=0&time=LOCAL&day1=5&month1=09&year1=2015&hour1=0). I may make a point to reference this data next time I'm doing some backpacking trip weather planning. 
* The [NOAA Hydrometeorological Automated Data System (HADS)](http://www.nws.noaa.gov/oh/hads/) also maintains a large number of weather stations. GNLC1 is included and you can search for it via the NWSLI ID search box. Here's a [detailed explanation from NOAA about HADS](http://www.nws.noaa.gov/oh/hads/WhatIsHADS.html).

##09/14/15 Update 

tl;dr: There are multiple weather station networks at play here, which unfortunately don't share data. 

Looks like the [Pinecrest lake](http://www.wunderground.com/weather-forecast/zmw:95364.1.99999) weather station I used for our forecast is actually located in [Cold Springs](http://www.wunderground.com/personal-weather-station/dashboard?ID=KCACOLDS1). It's a [Davis Vantage Pro2](http://www.davisnet.com/weather/products/weather_product.asp?pnum=06152) (and it even has a [webcam!](http://www.csclimate.com/) powered by some software from [Trixology](http://trixology.com/)). This appears to be just [one of 100,000+ non-professional weather stations](http://www.wunderground.com/about/data.asp) being utilized on Wunderground. 

###Does this matter? 

While Cold Springs, CA is very close to Pinecrest, it's not actually at Pinecrest Lake. In fact, on Wunderground there's another weather station called [MPNWC1](http://www.wunderground.com/personal-weather-station/dashboard?ID=MPNWC1), which is even closer being located in Strawberry, CA. However, when I click for the forecast for the area, it directs me back to the original "Sierras-Pinecrest Area" forecast. The takeaway: since Wunderground uses multiple weather stations to generate its proprietary forecast, no single weather station on their network is going to be the sole source of information (which makes total sense, weather patterns are geographically rather large). FWIW, this morning at around 6:30am there was an 8 ˚F temperature difference between the two stations (Cold Springs: 58.9 ˚F and Strawberry: 51 ˚F). 

However, it appears that Wundergound and HADS don't use each others weather stations. For instance, there is actually a [weather station on Pinecrest Lake (PNCC1)](http://weather.gladstonefamily.net/site/PNCC1), but I can't seem to find a weather service that includes its data (or Gianelli's for that matter). Granted, I wouldn't expect the CA Bureau of Reclamation or NOAA to use a private/amateur weather service's data, but I could definitely see Wundergound (or any of the other weather services) using HADS. That's a shame considering how valuable it would be to people in the area to use these stations to better prepare for their trips - especially for the Emigrant Wilderness.  

<a id="10" href="#01">[0]</a> I'd show the original forecast, but I didn't take a screenshot so I have to use historical data.

<a id="20" href="#02">[1]</a> In case anyone's keeping track, GNLC1 at Gianelli Meadow is located at an elevation of 8640 feet, Y Meadow Lake is 8750 feet, and Pinecrest Lake is 5640 feet. 
