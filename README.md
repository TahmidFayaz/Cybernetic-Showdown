# -Cybernetic-Showdown

# Arena Survival: Defender (Python & OpenGL)

## Core Mechanics

### Movement
* **WASD Keys:**
    * `W`: Move forward
    * `A`: Move left
    * `S`: Move backward
    * `D`: Move right
* **Bounding:** The player is confined to a square arena, with boundaries ranging from -50 to +50 on both the X and Z axes.

### Combat
* **Shooting:**
    * **Left Mouse Click** or **Spacebar** to fire a projectile.
    * There is a **0.5-second cooldown** between shots.
    * Bullets travel in a straight line in the direction the player is currently aiming.
* **Enemies:**
    * **Small Drones (Red):** 1 Health Point (HP), 10 points upon destruction. Fly randomly.
    * **Megatrons (Blue):** 3 HP, 100 points upon destruction. Emit bullets.
    * **Tanks (Grey):** 5 HP, 50 points upon destruction. Move on the ground and shoot purple projectiles at the player.

### Health & Power-Ups
* **Health:** The player starts with **100 HP**. The game ends when health reaches 0.
* **Medboxes (Red cubes with white crosses):** Collecting a medbox restores **25 HP**.
* **Shields (Cyan spheres):** Collecting a shield grants **5 seconds of invincibility**.

### Enemy Behavior
* **Drones:** Fly randomly within the arena and bounce off the arena boundaries.
* **Tanks:**
    * Move along the ground plane.
    * Fire projectiles at the player with a random interval of **3 to 7 seconds**.
    * Their turrets will track and aim at the player's current position.
* **Spawning:**
    * A new enemy will attempt to spawn every **5 seconds**.
    * There can be a maximum of **10 enemies** present in the arena at any time.
    * Small drones have a significantly higher chance of spawning compared to Megatrons and Tanks.

## Controls

* **V:** Toggle between **first-person** and **third-person** camera views.
* **P:** **Pause** or **resume** the game.
* **R:** **Restart** the game. This will reset all stats (score, kills, time) and clear all entities from the arena. This can be used after a game over or during active gameplay.
* **Q** / **Esc:** **Quit** the game application.
* **Mouse:** Controls the **camera aim** by tracking mouse movement.

## Scoring & Progression

### Points
* Destroying a **Small Drone:** +10 points
* Destroying a **Tank:** +50 points
* Destroying a **Megatron:** +100 points

### Stats Tracked
The game keeps track of the following statistics:
* **Total Score:** The cumulative points earned.
* **Tanks/Megatrons Killed:** The total number of tanks and megatrons destroyed.
* **Time Survived:** The total time the player has survived in the arena, measured in seconds.

## Game Over & Restart

### Loss Condition
The game ends immediately when the player's **health reaches 0**.

### Game Over Screen
Upon losing, a "**GAME OVER**" message will be displayed, and the gameplay will be paused.

### Restart
Pressing the **`R` key** will:
* Reset the player's health to 100.
* Reset the total score to 0.
* Reset the counts for tanks and megatrons killed to 0.
* Reset the time survived to 0.
* Remove all existing enemies, medboxes, and shields from the arena.
* Unpause the game, allowing the player to start a new round.


