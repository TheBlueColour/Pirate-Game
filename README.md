# Pirate Game

**Unit Name:** FGCT4016: Gameplay Design and Programming 25/26 

**Student Name:** Zuzanna Maria Pawelczyk

**Student ID:** 2506784 

**Total Word Count:** \[XXXX]

**API Reference Link:** \[URL]

**User Guide Link:** \[URL]

**Build Link:** \[URL or Embed]

**Video Demonstration Link:** \[URL or Embed]

---

## Abstract 

My goal is to create a 3D low-poly local multiplayer party game with three unique minigames with two other teammates working on the art side of the game, my personal task is to code a lobby, and the three minigames on Unreal Engine 5. My approach was to work out the very simpliest gameplay of the games before adding any complicated gamemodes.

The lobby would display how many wins each player has, as well as teleport each player into the minigames one by one, which in the final product i was able to do. I want every minigame to have a UI introducing to how the game works prior to playing the game. 

In the game the first minigame would a pvp map where the players can kill each other with a sword, a special gun that can be used once, block attacks with shields, avoid canon balls falling from the sky as well as collecting coins that can heal you in small amounts. The map would be inspired by an island, where the water is an instant death and a lava stream that slowly kills the player, once the player has died I want them to ragdoll and switch to a spectator mode. The map would also have areas where they can fall into a pitfull trap and loose a certain amount of health, to avoid the player getting stuck they can double jump to get out the trap.
In the final product I was able to create the pitfull trap, the sword and the coins to pick up for the player, I didnt have enough time to include a gun, a shield or avoiding canon balls. However, I was able to addd other environmental things like the water and the lava damaging as well as the ragdoll physics and spectator mode. 

The second minigame is a visual minigame where coins spawn in and the player is tasked with counting coins while ignoring other objects obscuring the coins and inputting the answer into the UI. There are six rounds and after six rounds the game will check for who is still left and give them both a point, if all but one player loose that one player gets a point. I was able to implement everything I wanted with this minigame. 

The third minigame is a QTE minigame where the player is given a direction they are required to click the correct button if they click the incorrect button they loose a life that is displayed on the ui, if the player clicks correctly they get a visual idication that they clicked correctly. Last player standing wins for all minigames. I was able to implement everything that i wanted for this minigame. 

---

## Research 

As a group we looked at different party games and focusing on their minigames, avoiding any minigames that would require online multiplayer as our game would entirely rely on local multiplayer. We looked at games such as Mario Party, Gang Beasts, Sea of Theives and Party Panic as well as I took certain minigame inspiration from Sonic Unleashed. 

### Game Sources

#### Party Panic:

Party Panic is a multplayer party game minigame with an initial release date of 2016 created by Everglow Interactive Inc. it's a game that is a party game similar to Mario party but with different minigames. This game manily inspired the lobby of my game. In Party Panic the players are in a lobby where the camera is pointed at all the players from a 3rd person where the players in a room and their points are displayed by a growing pillar beneath the player. I wanted to use a similar camera angle and but have the players movement be more limited within as well as have wins rather than points be displayed within the ui and not through a growing pillar. Despite the game being a party minigame we didnt explore the game's minigames as none are as interesting and didn't have as much potential to use as inspiration or they were inspired by Mario party already. 

![Example of Party Panic Lobby](image.png)

#### Mario Party:

We looked through different Mario Party games (created by Nintendo) and minigames for inspiration, excluding any minigames that would require for the minigames to have teams (like 2v2 or 3v1) we wanted free for all minigames. The minigame we landed on that gave us the most inspiration was a Drop Quiz from Super Mario Party. It's visual style minigame where a certain amount of
Toads or Paratroopas move across a screen with or without fruit and one player picks a question for the other three to answer. The players have to walk over to different spots where the number matches with how many moved across the screen until a certain amount of questions is asked. Despite this being a 3v1 minigame originally we were able to translate it into a free for all, where the players have to specifically look for coins on a screen and count them and then input them on their ui element. Players every time are instructed to count coins rather than different questions each time, but with different amounts of coins and different objects blocking the coins.

![Drop Quiz Minigame Mario Party](image-4.png)

#### Sonic Unleashed:

When looking for inspiration for the third minigame I was reminded of Sonic Unleashed for the Xbox 360 from 2009 made by Sega. How in the game there are certain segments that are Quick Time events. Upon clicking a random button that pops on screen you're able to progress in the game, and I took that as inspiration to make a rhythmn-like minigame, that you would be required to click any button the keyboard that pops up. I then realised that if I want the game to be compatible with a controller I had to reduce the buttons to just arrow keys like other rhythm game. 

![Example of Sonic Unleashed QTE](image-2.png)

#### Gang Beasts:

Gang Beasts released in 2017 by Boneloaf studios was our main inspiration behind map choices for our Pvp minigame. In Gang Beasts a unique aspect of the game is that the players are able to fight on maps that interact with the player, if its a train that drives past and can kill the player or break-able platforms underneath the players feet. With this I added things like the lava on the map being able to damage you over time if the player walks onto it as well as the entire water killing the player if they jump into it. On top of this I added traps, so it means the players have to be aware of the map and where they are walking as it will impact the game just like Gang Beasts does with it's maps. 

![Example of Gang Beasts map](image-3.png)

#### Sea of Thieves:

### Tutorial Sources

https://www.youtube.com/watch?v=yj04QBEjc38&t=2s - Levels and how to change between levels
https://www.youtube.com/watch?v=sWh1jgHb6Tw - Game instances so that i can keep information between levels.
https://www.youtube.com/watch?v=qVtoemgM7wI&t=633s - Help with the pick up system for the sword and gun
https://www.youtube.com/watch?v=JuzSB4Tg8BQ - help with finding how to make the mouse visible
https://www.youtube.com/watch?v=jkPxVScULh4 - Lock camera correctly in first person
https://www.youtube.com/watch?v=hsBzIQfYZw0&t=96s - Lock camera in first person but didnt help
https://www.youtube.com/watch?v=pWIJlsqli1w - Help with implementing hit scan which is just a line trace yay
https://www.youtube.com/watch?v=LfwQUGOQu2M&t=390s - Help with spawning items on a map but it didnt help and i just looekd how i did the spawning coins again
https://www.youtube.com/watch?v=tf0BvCl11lE&t=226s - Spawning swords on the map using a nav mesh instead of multiple spots
https://www.youtube.com/watch?v=AN2PbE26mAk&t=235s - Spectator 
https://www.youtube.com/watch?v=ef6SeknakeU&t=568s - how to make it multiplayer, didnt work, they did it differently to me
https://www.youtube.com/watch?v=2GYicrkCElA - Didnt work 
https://www.youtube.com/watch?v=s6DF1fkwTE8 - Countdown timer
https://www.youtube.com/watch?v=RdaAVTMIg08&t=323s - was unable to make this work



Where I got the Arrows from:
 
https://www.i2symbol.com/symbols/arrows

