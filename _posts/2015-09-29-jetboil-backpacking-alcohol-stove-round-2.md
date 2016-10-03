---
layout:     post
title:      Jetboil backpacking alcohol stove - round 2
date:       2015-09-29 
summary:    More fun with fire
tags:  
  - backpacking 
  - ultralight gear
  - stove
allow_comments: TRUE
---

In [a previous post](http://robm.xtz/blog/jetboil-backpacking-alcohol-stove/) I showed how a Fancy Feast/Super Cat stove is compatible with a Jetboil Minimo stove pot. I mentioned I would put up some numbers when I got around to doing a test boil, and here we are.

## Testing

The setup itself is straightforward: measure how long it takes to bring two cups of tap water to a rolling boil using 1 oz of fuel. I used denatured alcohol as it was most available <a id="00" href="#01">[0]</a>. 

{% include image.html url="/images/jetboil-alcohol-stove-v2-7.jpg" description="The Jetboil MiniMo/Fancy Feast setup with another Fancy Feast reject in the picture fore scale." %}

Overall, I was pleased with how the flux ring seemed to keep the flames from reaching up around the sides of the pot. It's not good enough to be able to leave the stock Jetboil lid on there (I tried), but I wasn't expecting that anyways. 

### Results
* Two cups tap water (room temperature)
* 1 oz denatured alcohol
* Time to rolling boil: 10:00
* Total burn time: 12:55

{% include image.html url="/images/jetboil-alcohol-stove-v2-3.jpg" description="The Jetboil Minimo working well with the Fancy Feast stove. Notice how close the bottom of the pot is to the table." %}

This result is ok, but I wasn't really impressed. Overall I found the setup messy since it was entirely too easy to spill alcohol when pouring it into the stove, as well when placing the pot on top. I was pretty sure I could do better. 

##Let's dissect a Jetboil stove

{% include image.html url="/images/jetboil-alcohol-stove-v2-9.jpg" description="The Jetboil stove taken apart. Refreshingly easy to dissassemble/reassemble." %}

{% include image.html url="/images/jetboil-alcohol-stove-v2-11.jpg" description="The Jetboil Minimo, Fancy Feast can, and removed top from the Jetboil stove." %}
{% include image.html url="/images/jetboil-alcohol-stove-v2-2.jpg" description="Fancy Feast can with the top ring removed." %}
{% include image.html url="/images/jetboil-alcohol-stove-v2-10.jpg" description="The Jetboil Minimo combined with the Fancy Feast can as well as the removed top from the Jetboil stove." %}

At this point I had a clean looking setup, but all my attempts to light it led to the flame getting snuffed out due to lack of oxygen. One of the ways you can get around this is to build a wick. 

##Let's build a wick
{% include image.html url="/images/jetboil-alcohol-stove-v2-1.jpg" description="Fancy Feast + tomato paste can + wick aftermath. That charred black gossamer is the lining to the tomato paste can (likely to prevent the tomato from reacting with the can). The wicking material is a fiberglass strip is found in the shed." %}
{% include image.html url="/images/jetboil-alcohol-stove-v2-4.jpg" description="Fuel being forced to spill out of the fancy feast wick due to pressure buildup between the tomato paste can and the pot bottom." %}
{% include image.html url="/images/jetboil-alcohol-stove-v2-5.jpg" description="Everyone loves a good fail photo. The failed stove wasn't imperiling anything, so I just let it burn out." %}

##Postmortem

Things did not go well here. In fact, I was rather close to pulling the pin on my fire extinguisher and ending the experiment, but luckily I was able to let the stove burn itself out <a id="10" href="#11">[1]</a>. So what happened? 

I essentially had two chambers connected by who semicircular holes in the base of the tomato can. The space between the outside of the tomato can and the inside of the fancy feast can was the wick. The whole stop of the stove sat flush against the underside of the Mini-mo pot. Fuel sat in the bottom, but saturated the wick. As the stove initiall burned, the flame pattern was great. However, as the whole system heated, I'm fairly certain that the air trapped on the inside of the tomato can couldn't escape. So naturally, if we assume [PV=nRT](https://en.wikipedia.org/wiki/Ideal_gas_law) and a fixed volume, then as the temperature of the system increases the pressure must also increase <a id="20" href="#21">[2]</a>. Since the air has nowhere to go, it exerts increased pressure against the fuel. Since the fuel fully saturated the wick, this resulted in the wick excreting liquid, unburnt fuel down the sides of the stove. The more the system heated up, the more fuel was pushed out. This naturally resulted in my entire setup being engulfed in flame. 

So how do you fix this problem? Looks like what you need to do is increase the height of the inner can and pop a hole in the top, [just like this guy's setup](https://www.youtube.com/watch?v=p2fPIvyme9I). 

##Conclusion

I'm done with this experimenting for now. If I pick this project up again, I'll likely replicate the youtube setup to ensure that my understanding of the system is correct, and the re-evaluate the project as a whole. 


<a id="01" href="#00">[0]</a> If I get more serious about using alcohol stoves, I'll probably look into sourcing ethanol.

<a id="11" href="#10">[1]</a> This is often cited as the main drawback to using an alcohol stove. If something goes wrong, like a fuel leak, then you've got quite the mess on your hands. I wouldn't say enough to start a forest fire (especially if you're following general safety guidelines), but certainly a big waste of fuel and time. 

<a id="21" href="#20">[2]</a>Of course, as the air pushes fuel up the wick the volume of the space increases (which would reduce pressure), but I'm declaring this increase negligable when compared to the large increase in temperature (especially as the spilled fuel ignites and engulfs the entire stove in flames).