---
layout: post
title:  "Technical Experiment #4"
date:   2021-10-10 17:02:41 -0400
categories: jekyll update
---

This week I wanted to start off by figuring out what kind of game I wanted to do. I wanted to do a multiplayer fps game, but with the issues I was having with Photon, I needed a solution. I decided that I was still going to design a multiplayer game, but in place of players implement AI enemies to fight. This week I also need to develop a map, as the current map is just an open field and is not very fitting for this theme. Lastly, I wanted to start implementing the 3 new analytics from last week. If I have time I also wanted to implement a couple new weapons.

I started by working on the map, as without it I will have a harder time testing the enemy AI. I implemented NavMesh Obstacle spawning so that when the terrain rises and falls the enemy recognizes the new hills. I removed the random hills rising up. I added lightning that blasts the earth when the ground rises. 
<br> ![](https://i.imgur.com/Yyy3LEJ.gif)
<br>Originally I started with a large open map, throughout development though it started to feel more like a battle royal map and this was not the style of game I wanted. Eventually, I decided to reduce the map size into a sci-fi city map. The fog acts to limit the size of the city and made the playable area much smaller. In the future I want the player to be able to walk into the fog and take damage when they enter the fog. For now there is just a collider. 
<br> ![](https://i.imgur.com/GtuiQIw.png)
<br>I added 3 space ships in the fog that the lightning originates from. The idea is these ship can add a sort of story. Basic story is that there are 2 teams, the aliens and inhabitants. The player controls an inhabitant, and the aliens are trying to kill the inhabitants. The aliens can continue to respawn up until the end and the inhabitants get 1 life. Idea for a gamemode is teams swap after all inhabitants are killed. You gain points for each alien you kill as an inhabitant. The team that lasts the longest gets the most points. Next week I want to implement this gamemode, also I want to create friendly AI to play alongside player. 
<br> ![](https://i.imgur.com/NNqTwlA.png)
<br>I added a few more enemies, found an enemy "alien" model online that I could use for the characters to replace the capsule. I also implemented the walk animation to show enemies walking. 
<br> ![](https://i.imgur.com/pSdrb4N.gif)
<br>I did run out of time and was not able to implement the analytics but I did come up with solutions to the questions I asked last week. Currently, the guns shoot bullets. I want to replace these with lasers. The lasers will be different colored based on weapon (will match analytic screen). Weapons will run out of ammo over time. The game will drop ammo when you kill an enemy. This ammo type will start off being based on what the enemy was using. Once the game has collected enough data from the player, the ammo will be based on which weapons are being used least and what weapon the enemy is using.

I also want to introduce random loot drops. These will be deployed from the alien space ships. If the game detects that inhabitants aren't looting these crates then there will be a chance an alien drops a loot flare on death. This flare will allow the player to summon a loot drop at their location. 

Lastly, I plan to monitor where aliens are dying. If aliens are dying in an area, the game will change the spawn location to try and get aliens to enter a new area and not push the same place. If even after the spawn point changes aliens continue to die in a certain spot one of the 3 space ships above will crash into the planet. Maybe a inhabitant cannon from off the map can be seen shooting it down. The ship will crash into the spot and add an obstacle to the NavMesh to keep AI players away and will block the area so real players will not be able to go there either. 

<br>Time Log:
<br>Tuesday: 0
<br>Wednesday: 0
<br>Thursday: 1 hour- NavMesh Obstacle Spawning
<br>Friday: 3 hours- Map Development, finding models. Started with much larger map and found a ton of models online to populate.
<br>Saturday: 2 hours- Map Development cont. Added more models to map and messed with terrain.
<br>Sunday: 4 hours- Map Development cont. Decided map was too big for style of game. Found 1 model for entire city, implemented colliders, NavMesh, and sized fog to appropriate size.
<br>Monday: 3 hours- Enemy AI bug fixes, models, and animations. Started analytics but was not able to make real progress. 
