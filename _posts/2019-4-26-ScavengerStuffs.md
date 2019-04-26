---
layout: post
title: "Scavenger Stuffs"
date: 2019-4-26
excerpt: "2019 Game Challenge (April) A mobile game based around scanning pendants against hidden stuffed animals to collect characters in-game."
tags: [game,unity,scavenger,stuffs,rfid]
comments: false
---
<center>
<div markdown="0"><a href="https://play.google.com/store/apps/details?id=com.Lightmoon.ScavengerStuffs" class="btn btn-success"> App Download</a>

{% capture images %}
    https://lh3.googleusercontent.com/pvUjQFw5DvhzewN8KFAlhiXZkQmqtC51Q0qZ8hHl1DIqitMrWr2Y9ukd8K7nyM95yIY=w5120-h2660-rw
{% endcapture %}
{% include gallery images=images caption="" cols=1 %}

</center>

### Summary

Built as part of the Lightmoon 2019 Game-A-Month challenge, and for the Wearable Technology course at UW-Madison. 

Scavenger Stuffs’ goal is to bring wearable technology down to a more accessible level, and to help get everyone exploring!

Scavenger Stuffs was built around the idea to make wearable technology cheap and accessible. By pairing a medium expense, a free mobile app, and a $1 player pendant together, the entire game helps create a unique and fun twist on scavenger hunts.

The stuffed animals are intended to be bought at-cost for manufacturing ($20-$30) by local business, or donated to libraries and museums. Each stuffed animal is a standalone unit in the game, complete with its own unique design in real life, and in the mobile app.

Once a player finds a location which distributes pendants (Decorative tags which cost <$1 to create), they use the pendant to register for an account on the mobile game. From that point on, players can scan their pendants against any stuffed animal they find, and it will be added to their game’s account.

### Screenshots

{% capture images %}
	https://lh3.googleusercontent.com/X2rZwjtRTDNQGdrph67-rN4QIb76Kwhcafso6XAPVZ6SfL7KSr9e1UqZ9cMWWcMBgYhE=w5120-h2660-rw
{% endcapture %}
{% include gallery images=images caption="Scavenger Stuffs Gameplay" cols=3 %}

### Development Information

Stuffed Animals
Each stuffed animal has a microprocessor (Raspberry Pi Zero W), an RFID Scanner, and a power source. When a pendant is held against the RFID scanner, the username stored on the pendant is updated with the animal in our database, ready to be added to the game. The total components used to create the animals total to between $20-$30 each.
•	Pendants
The pendants are simple RFID tags that have been prewritten with a username that can be registered in the game. Pendants are made to be cheap, costing under a dollar to buy and ready for distribution in only a few minutes on the production-side.
•	Mobile Game
The game itself was made using Unity, and is available for Android devices. It wires into a backend server of Gamesparks for login/registration. 


#### Software Used: 

***Mobile Engine & Dummy Engine:*** Unity
***Mobile Backend:*** GameSparks
***Stuffed Animal Internals:*** RFID-522 Reader/Writer, RaspberryPi0W, Raspbian OS, Portable Charger
***Pendants:*** RFID Tags wrapped in baking clay
