#Space Kerfuffle!

##Project Overview

For this project, you will make a top down space-combat game, similar to arcade classics such as Space Invaders, Demon Star, or Galaxian.  Players will control a spaceship and face off against swarms of flying baddies in a vertically scrolling levels.  No space combat game would be complete without a screen full of projectiles flying back and forth!

You will create a LibGDX project, implement a level loader and asset manager to load all the relevant data and assets for the game, and write the code for the game itself.  Art assets will be provided for you, but you're free to use your own if you want!  In the game, enemies should spawn at planned intervals and execute basic offensive behavior while the player dodges and weaves among incoming projectiles while firing off salvos of their own.  At the end of the level, you will create a showdown with a boss.

##Completing the Project

You will take the following steps to complete the project.

###Basic Structure

* Create a LibGDX project and implement the basic framework for a game (using the Game class, Screen interface, Viewport class, etc).

* Create whatever classes you deem necessary, though we recommend at least a class for the player's ship, for enemies, and for different projectiles.

* Load level data from a JSON.  (Optional: create the JSON using the Tiled map editor.)

* Load all art assets in an efficient way using an AssetManager.

###Gameplay

* The player can move their ship using the arrow keys and fire projectiles (lasers) with a button.  On mobile, the ship will follow the player's finger and be constantly firing.

* Enemies spawn at regular intervals according to the level data you created and loaded, and execute simple attack patterns.  The minimum requirement is that enemies move down the screen and fire projectiles below them, but for a better feel, we recommend you give the enemies behaviors such as strafing back and forth across the screen, firing projectiles in different directions or directly at the player, and similar.

* You must implement 2D collision detection for all the projectiles, destroying enemies or the player when they are hit.  The player should have some fixed number of lives before they lose.

* At the end of the level, program a simple boss battle against a powerful foe.

###Visual Component

* We provide art assets for the player ship, enemies, lasers, missiles, explosions, and a boss.  These should be rendered using a SpriteBatch.

* You must implement simple animations for ships and explosions using LibGDX's Animation class.

* Include a HUD that displays the player's score, which goes up when they kill enemies.  Also display their life count, and any other pertinent information such as secondary weapon ammunition if you include it.

###Bonus Challenges

* Give the player a secondary weapon that behaves differently, such as missiles or bombs.

* Give enemies more in depth movement patterns and attacks, such as symmetrical formations, complex flight patterns, or homing or aimed shots.

* Add powerups such as extra ammunition for secondary weapons, improvements to the primary weapon, and extra lives.

* Include music and/or sound effects.