---
layout: post
title:  "Technical Experiment #8"
date:   2021-11-15 17:02:41 -0400
categories: jekyll update
---
Last weeks build had a significant number of bugs that I needed to address. To begin when the game restarted after the player lost the CPU froze upon attacking and I spent a decent amount of time debugging before realizing one of my functions in the scoreboard was not functioning properly. Additionally, I felt the rifle was not firing at a proper rate and adjusted the rate of fire to properly balance it. This led me to my next bug. I discovered the weapons were not always firing and sometimes bullets were disappearing without hitting anything. Upon doing some digging I realized the bullets were colliding with each other out of the rifle and was able to quickly fix this.
<br>![](https://i.imgur.com/6Hjcfbb.gif)
<br>Upon completing the weapon fixes I focused on fixing smaller bugs I found within the AI scripts and cleaned up my map a little bit. I found a couple more holes in the navmesh that needed patching and I adjusted the sky, removed the upper fog, and added in some dynamic clouds to make the game feel more alive. I think the clouds need to be made a bit more cartoon style but for now they work. Additionally I adjusted the end screen to show the players score no matter the outcome of the game and not only the highest score.
<br>![](https://i.imgur.com/lWnop65.jpeg)
<br>On Thursday I did a lot more bug fixes and playtesting. No major bugs popped out, but some minor ones were found and quickly patched.
<br>
<br>Finally, I revisited some of the ideas that were mentioned during class last week. I implemented a "shield" around the Ally players to build on the reason for them to have more health. When their health reaches 2 (the default health for enemies), the shield disappears and they are the same as enemies. 
<br>![](https://i.imgur.com/JqjGtcV.png)
<br>Additionally I removed the terrain from my scene and decided to implement a tractor beam that lifts players into the sky to build on the spaceship idea. I implemented fall damage so that if the player allows the tractor beam to lift them up too high they will die, but moving in any direction out of the beam will drop them. 
<br>[Video to see tractor beam](https://i.imgur.com/6TxRIbq.mp4)
<br>You can download the new builds [here for Windows](https://drive.google.com/file/d/1XaBM19eYMxONy3YMMoUpbDQY3BbbywvC/view?usp=sharing) or [here for Mac](https://drive.google.com/file/d/1-Z3oXxfXYYHjh43oNBlgvwsfy50trxjS/view?usp=sharing). Pressing the O key closes the application as I haven't implemented a quit button yet, and the tractor beam activates after 2 kills in the same spot currently to showcase the feature but in the final build it will be around 10. Next week I will be implementing a shotgun type weapon, adding more enemies so the game is not as slow, and I will be putting a lot of work into the map to make it feel less open.

<br>Time Log:
<br>Tuesday: 2 hours- Bug Fixes and weapon balancing
<br>Wednesday: 3 hours- Bug Fixes, scoreboard, and sky
<br>Thursday: 2 hours- Bug Fixes and playtesting
<br>Friday: 0 hours
<br>Saturday: 0 hours
<br>Sunday: 0 hours
<br>Monday: 5 hours- Bug Fixes, Ally Shields, and tractor beam
