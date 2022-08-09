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
Getting the AI to want to take over the world was challenging as the return on investment is low.

### Most interesting
The parts of the game that really shine and show off my programming ability

### Reflection on Learning
What was the most important this I learnt in the process.  One way to frame this is to look at things you struggled with and think about how you solved those and if that solution is **transferable** to similar situations.

Reflections can be at multiple levels.  Specific things that you learnt about the code, things you learnt about programming in the environment, things about programming in general, things about learning, or even things about how you value different aspects of your life. We expect you to cover the general programming and learning reflections based on specific examples but showing that you have generalised from those a more interesting lesson.

You need to edit this readme to discuss your project. .  If you are doing a technology then you need to change the header above.  Edit <your name> to be something like Simon McCallum

The assingment description is in [Assignment 1 markdown](assignment1.md) 
