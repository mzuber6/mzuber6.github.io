---
layout: post
title:  "Technical Experiment #6"
date:   2021-11-01 17:02:41 -0400
categories: jekyll update
---
I started this week out by fixing numerous bugs in my code. There were some slight issues with how the weapons worked, how ammo was limited, and how the spawn points changed. I cleaned up these bugs and made sure things were working as imagined. For the ammo limiting, I decided instead of limiting after 100 rounds were fired, to instead use a formula that altered the number based on the amount of damage the weapon does. A weapon that deals more damage will limit after less rounds are shot while a weapon that deals little damage will have more ammo provided. Additionally when the game was checking for other types of ammo to drop when limiting, it was just looking at what weapon had fired the least, but it needed to be put through that formula so weapons that don't deal a lot of damage are provided ammo.
<br>
<br>I also updated the spawn points and made it so that when selecting a new spawn point, the game raycasts from the new point to the player to verify that the player can not see the enemy spawn point on first use.
<br>
<br>Next, I worked on the game play itself. To begin I gave the enemies a way to randomly select locations on the map to travel to. The enemies will walk around the map now looking for the player until they spot them. If the enemy loses sight of the player, it will travel to the last known location and if the player is not found will begin searching the map again. Additionally, I began working on the ship crashing but stumbled across multiple bugs when doing so. Selecting a location for the ship to crash has been the main issue, and I need to brainstorm how I would like to approach this next week.
<br>![](https://i.imgur.com/0FZCNVT.gif)
<br>I then developed AI teammates that wander around the player. The AI stays within a distance of 25 but is constantly roaming. When an enemy is spotted they will target them. If the teammate doesn't have an enemy to target it will return to the player. 
<br>![](https://i.imgur.com/M5vNt56.gif)
<br>I implemented the infection style game mode and made it so when the player or teammates die, they join the Alien team. Additionally I designed a simple UI that shows player health, and teammate health. This way the player knows when their teammates are about to die. I do want to add in player names above the teammates so that the player can tell which health corresponds to which ally and where the ally is. 
<br>![](https://i.imgur.com/EvCUE2N.gif)
<br>Time Log:
<br>Tuesday: 0 hours
<br>Wednesday: 0 hours
<br>Thursday: 0 hours
<br>Friday: 1 hour- Bug fixes
<br>Saturday: 6 hours- Bug fixes, enemy AI, and attempted to work on ship crashing
<br>Sunday: 3 hours- Teammate AI
<br>Monday: 4 hours- Infection style game mode, UI, and bug fixes
