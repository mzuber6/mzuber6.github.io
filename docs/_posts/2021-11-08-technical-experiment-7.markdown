---
layout: post
title:  "Technical Experiment #7"
date:   2021-11-08 17:02:41 -0400
categories: jekyll update
---
I started this week out by messaging a few people on LinkedIn to see if they were open to meet to discuss my topic but have not heard back from any of them. I then created a start scene for the game to allow the player to click start instead of just throwing them into the game. 
<br>![](https://i.imgur.com/V89NwDm.png)
<br>I then moved on to fixing numerous bugs in my project, to begin there were numerous flaws with the AI navigation and navmesh. The mesh I was using for the city seemed to have holes in it and this was causing the navmesh to have holes. I spent some time this week fixing these holes in order to correct the navmesh. Additionally I realized the roofs of the buildings were included in the navmesh and occasionally the AI would try to find a path to the roof which was not possible. This would cause the AI to sit still and not move. I added in a navmesh obstacle that encompasses all the building roofs so the AI does not attempt to route to the roofs. 
<br>![](https://i.imgur.com/2Hum3dr.png)
<br>Next I implemented the player respawn mechanic that turns the player into an enemy. This allows the game to be a true infection mode game and not just end when the player dies. I also completed the game loop and implemented a game over scene for when the last "Ally" or inhabitant of the planet dies. Additionally I implemented a highscore that is displayed on the end screen. Players and CPU get points by getting kills.
<br>![](https://i.imgur.com/gMlq5Ya.gif)
<br>I then spent the majority of the week fixing multiple bugs that popped up in my build. You can download to play my first build [here for Windows]() or [here for Apple](), though it is not bug free and has a few flaws.

<br>Damage * Rate of fire
<br>Time Log:
<br>Tuesday: 1 hour- Messaged stakeholders on LinkedIn
<br>Wednesday: 0 hours
<br>Thursday: 0 hours
<br>Friday: 1 hour- Start Scene
<br>Saturday: 3 hours- Bug fixes (AI navigation, holes in navmesh, holes in city mesh)
<br>Sunday: 3 hours- Player respawn
<br>Monday: 4 hours- End Game/Complete Game Loop and Bug fixes
