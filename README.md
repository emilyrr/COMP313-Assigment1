# COMP313 Assignment 1 
## Emily Rhodes-Robinson 300526534

## The Floor Is Lava!

[Gameplay video](https://www.youtube.com/watch?v=WB6w7ovocpk)

## Description
The Floor Is Lava is a digital reindition of the classic kids playground game! The aim of the game is to collect all the coins on the level by jumping from platform to platform without touching the lava.


### Main mechanic
The player is viewed from a third person perspective and the direction of movement is controlled using the 'w','a','s','d' keys. The player can jump by pressing the 'space' bar, once for normal jump or twice for double jump. They can also sprint by pressing 'shift' or crouch by pressing 'ctrl'. There are transitions between the jumping, crouching and running/walking states to ensure the state can be entered from the current state i.e. you can't jump directly from a crouch .

Collecting the coins is one of the main actions in the game. The coins are classed as Actors with a sphere collision property which triggers an incremental increase in points upon collision. Once the player collides with a coin, the coin makes a clink sound and dissapears to indicate that it has been collected. Once all of the coins are collected, the game is over and the final 'Game Won!' screen is displayed with the option to restart.


### Development difficulties
One difficulty I had was implenting the character animation blueprint on the different movements. I added animations for the different speeds of moving - idle, walking, running and sprinting - as well as idle and walking crouch. I encountered a lot of confusing problems which required a lot of trouble shooting with my limited knowledge of the unreal engine! However, they were great learning curves which have helped me to gain a better understanding of how the system works.

The biggest challenge for me was just familiarising myself with the unreal engine software as there were multiple times where it would completely crash and lose all my progress from half a days worth of work. It was a very good reminder to regularly commit and push my work to github. 

Also being limited to just Te Aro campus emphasised the importance of time management... I definitely underestimated how long seemingly simple tasks would take to perform!


### Most interesting
The player's interactions with the objects in the game such as the coins and lava are really great aspects that are essential for the game play and communicate with the player and UI HUD displays too. 

I created the lava material myself by combining the fire and rock materials provided in the starter content, making them dynamic by adding a speed factor in the x axis, and adjusting the emissive colour to flucutate brightness with a sine wave pattern. This creates a dynamic flowing lava appearance. I would love to continue developing the world environment to have a more jaggered ground and a change in the material where it collides with rocks and solid objects, such as an explosive splash.

When the player touches/collides the lava, it damages the health of the player at a damage rate that depends on the playing mode (normal or hardcore) and this is displayed on the gameplay HUD screen. Once the health bar reaches zero, the player "dies" and the game is over which is signified by the game status screen that is triggered with the string parameter "Game Lost!" to be displayed and a button to restart the level.

### Reflection on Learning
_What was the most important this I learnt in the process.  One way to frame this is to look at things you struggled with and think about how you solved those and if that solution is **transferable** to similar situations._

_Reflections can be at multiple levels.  Specific things that you learnt about the code, things you learnt about programming in the environment, things about programming in general, things about learning, or even things about how you value different aspects of your life. We expect you to cover the general programming and learning reflections based on specific examples but showing that you have generalised from those a more interesting lesson._

The idea for my game stemmed out of the functional elements that I had been working on incorporating. The first was the task of making the player interact with an object; this is where the coin idea came, and then editing the control system  inspired the idea of "The Floor Is Lava" - a familiar game but balanced with a reimagination of adding the coin collection task. I learnt a lot about balancing different aspects of the game, especially complexity vs clarity. I had so many ideas of how the game could be extended, for example adding a countdown timer that the user had to complete the game within, or adding more tasks or powerups, however all these elements added an extra complexity in both the gameplay and the background coding, therefore compromising the clarity. I discovered a better solution would be to incrementally add these details as the levels got higher so that the user can understand the key concepts of the gameplay initially, and then build on these slowly as their confidence and ability increased.

I thouroughly enjoyed learning to use blueprints as they are a great visual representation of what the code is doing and as a visual learner, this is a big win for me! Next time I will defintiely focus on implementing more functions to increase the efficiency of the code. I can see how at a higher level, the blueprint code would become extremely cluttered and unnessicarily repetitive without more sufficient use of the function blueprints.

Whilst it always took me a significantly long time to learn how to do something the first time, it became much quicker once I had to redo the same tasks or apply that knowledge to another aspect of the project. It took me a while to get into the project, but I have a much better understanding of the basics in UE5 now which I'm excited to build upon for the next projects.
