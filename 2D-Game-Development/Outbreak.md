#Outbreak

##Project Overview

For this project, you will make a simple game reminiscent of classic Atari arcade game *Breakout*.  Players will control a platform at the bottom of the screen that moves from side to side to intercept a ball that will bounce on impact.  The goal is to stop the ball from falling past your platform and deflect it into various blocks in the upper half of the screen.  When the ball collides with a block, the block is destroyed.

You will create a LibGDX project, implement a Screen, draw the game objects using a ShapeRenderer, and program the controls and real-time motion of the ball.

##Completing the project.

Completing the project consists of the following tasks.

* Make a LibGDX project using the project generator tool.

* Create a play screen using the Game class and Screen interface.

* Write a render loop that displays all the game objects, including the player's platform, the ball, and the blocks, using  ShapeRenderer.

* Program the gameplay, including:
** Polling for input to move the platform (arrow keys for the desktop build, and using the accelerometer on Android)
** Moving the ball in real time and programming its bounce behavior.
** Collision detection that makes the ball bounce when hitting a wall or block or the player platform, and destroying blocks on hit.

* Bonus challenges:
** Implement a Score that goes up as the player destroys blocks.
** Add a start screen, Game Over screen, and/or win screen.
** Implement different difficulty settings (eg the ball moves faster, there is a time limit, blocks take multiple hits).
