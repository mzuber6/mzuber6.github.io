---
layout: post
title:  "Technical Experiment #5"
date:   2021-10-25 17:02:41 -0400
categories: jekyll update
---

This week I set out to implement the technical items from 2 weeks ago. I started by implementing the lasers in place of the bullets and the limited ammo. The lasers are colored based on color in pause menu (Sniper=yellow, rifle=red). I start both guns with 50 ammo, though this may need to be adjusted in the future due to the fire rates. 
<br>![](https://i.imgur.com/ysq3Tmy.gif)
<br> Next I added in the ammo drops that come from enemies and made it so the player can pick up the drop by walking into it. As the game collects data it changes the type of ammo. It waits for the player to have fired 100 rounds from a weapon with 100+ ammo still before limiting that weapon. If the player has fired 100+ rounds but has less than 50 ammo the game does not limit the ammo drop.
<br>![](https://i.imgur.com/aehAQtR.gif)
<br> Additionally, I added in the flare that allows the player to call in ammo drops. Initially the flare has no chance of spawning. As the game goes on random ammo drops spawn in. If after 1 minute a drop isn't picked up, it despawns and slightly increases the chance a flare is spawned in. 
<br>![](https://i.imgur.com/STMjOGm.gif)
<br>Once the flare spawns in, the odds of a flare spawning is reset to 0. 
<br>![](https://i.imgur.com/HaVYPyj.gif)
<br>Lastly this week I implemented the spawn point change I previously mentioned. When aliens die in an area more than a variable amount of times the spawn rotates to a different pre-set location. This is calculated with the following equation, and moves the spawn when the statement is true: 
<br>
<br>(times alien has died) * (multiplier constant) / (distance from spawn alien died) > 3
<br>The multiplier constant is set to 50 for my usage and represents the size of the spawn area
<br>
<br>What this statement does is moves the spawn if the aliens are having issues in a location that is spawn related. For example, if aliens keep dying very far away, this may not have to do with spawn location and may just have to do with players camping so we are more hesitant to change the spawn location, waiting until the aliens have significantly more deaths. If the aliens die at their spawn though, they change their spawn point with very few deaths to counter players spawn camping. The new spawn point is then randomly selected from a list of spawns that are at least 200 units apart from the current spawn point. 
<br>![](https://i.imgur.com/APbORXC.gif)
<br>Unfortunately I fell pretty under the weather on Sunday and Monday and was not very productive due to being bedridden both of these days. I have not yet implemented the ship crashing previously mentioned to block off a path but hope to get this implemented early next week. Next week I plan on putting in roughly 18 hours to make up for this week. I want to accomplish a couple different things next week. To start, I want to reach out to more stakeholders as I haven't heard back from any from last week. Next, I want to implement the ship crashing and work out any bugs with the spawn point changes. Then, I want to finish implementing the infection style game mode. This means creating AI teammates, setting up the inhabitant deaths to turn them into aliens, and setting up player health and stats with a UI to share these stats. This way I can better get peoples opinion of the implementations and see what players like or dislike.

<br>Time Log:
<br>Tuesday: 0 hours
<br>Wednesday: 1 hour- Lasers and limited ammo
<br>Thursday: 0 hours
<br>Friday: 3 hours- Ammo drops from enemies and terrain adjustments
<br>Saturday: 4 hours- Flare implementation and spawn point rotation
<br>Sunday: 0 hours
<br>Monday: 30 mins- Ship crashing started
