---
layout: post
title:  "Technical Experiment #3"
date:   2021-09-29 17:02:41 -0400
categories: jekyll update
---
This week I started by sitting down with Nathan Hanish from Stardock. On Tuesday and Wednesday I spent roughly an hour preparing questions for the 15 minute interview. During the interview I asked him many questions relating to analytics and how they are used in the industry and asked him if he had any suggestions relating to the topic. He said there are 2 groups that look at analytics, the marketing team and developers. He said he has done work with increasing and decreasing the difficulty of the AI but nothing in terms of map changes. One recommendation he gave was to tell players upfront that the AI is using player data, via a button that players click to consent to feedback being recorded. Players can be very sensitive to AI, when it feels as if it is cheating. Another tip he gave was to make sure players are challenged and engaged, some implementations of what I am working on could be very frustrating to players.

To start this weeks technical experiments I tried to get Photon to work so I could have a multiplayer game. Instantly I ran into a ton of issues and was struggling to get Photon to work. I had lots of syncronization issues and was really struggling to just get the game to work multiplayer. I decided to scrap Photon and realized it was going to take too much time to implement and would be better to design a single player AI, or find one online that could play the fps game with the player. Sunday I worked on fixing some bugs that were present for about 2 hours. The first being bullets randomly spawning in wrong spot. This was because I had a rigidbody on the player accidentally in addition to the character controller component. The second bug was dealing with how the terrain moved up and down. This is now much cleaner. There was a lot of other small corrections that were made. AI script that would move toward the player, I implemented player health as well, and a death/respawn mechanic for the AI. 


Time Log:
<br>Tuesday: 20 minutes- Planning for interview
<br>Wednesday: 1 hour- Planning for interview, interview, and summarizing interview
<br>Thursday: 0
<br>Friday: 2 hours- Photon work
<br>Saturday: 0
<br>Sunday: 4 hours- Bug Fixes, AI to play against
<br>Monday: 5 hours
