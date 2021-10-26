---
layout: post
title:  "Technical Experiment 5"
date:   2021-09-06 17:02:41 -0400
categories: jekyll update
---

This week I set out to implement the technical items from 2 weeks ago. I started by implementing the lasers in place of the bullets and the limited ammo. The lasers are colored based on color in pause menu (Sniper=yellow, rifle=red). I start both guns with 50 ammo, though this may need to be adjusted in the future due to the fire rates. 
<br>![](https://i.imgur.com/ysq3Tmy.gif)
<br> Next I added in the ammo drops and made it so the player can pick up the drop by walking into it. As the game collects data it changes the type of ammo. It waits for the player to have fired 100 rounds from a weapon with 100+ ammo still before limiting that weapon. If the player has fired 100+ rounds but has less than 50 ammo the game does not limit the ammo drop.
<br>![](https://i.imgur.com/aehAQtR.gif)
<br> Additionally, I added in the flare that allows the player to call and ammo drop. Initially the flare has no chance of spawning. As the game goes on random ammo drops spawn in. If after 1 minute a drop isn't picked up, it despawns and slightly increases the chance a flare is spawned in. 
<br>![](https://i.imgur.com/STMjOGm.gif)
<br>Once the flare spawns in, the odds of a flare spawning is reset to 0. 
<br>![](https://i.imgur.com/HaVYPyj.gif)
<br>Lastly this week I implemented the spawn point change I previously mentioned. When aliens die in an area more than 5 times the spawn rotates to a different pre-set location. I have not yet implemented the ship crashing to block off a path but hope to get this implemented early next week. The following Gif demonstrates the alien spawn rotating if the rotation occured after 2 deaths.
<br>![](https://i.imgur.com/APbORXC.gif)
