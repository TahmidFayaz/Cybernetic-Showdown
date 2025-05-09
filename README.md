# -Cybernetic-Showdown

# Arena Survival: Defender (Python & OpenGL)

## Objective

Survive for as long as possible by strategically defeating waves of diverse enemies while effectively managing available power-ups. Accumulate points by destroying hostile entities and enhance your offensive capabilities by upgrading your weapon to increase its firepower.

## Core Mechanics

### Movement
* **WASD Keys:**
    * `W`: Move forward
    * `A`: Move left
    * `S`: Move backward
    * `D`: Move right
* **Mouse:** Look around the environment and control your aiming direction.
* **Bounding:** The player is confined within a square arena spanning 100x100 units on the X and Z axes.

### Combat
* **Shooting:**
    * **Left Mouse Click** or **Spacebar** to fire your weapon.
    * **Gun Levels:** Your weapon's damage increases by 1 for every 100 points you score (e.g., Level 1 deals 1 damage, Level 2 deals 2 damage, and so on).
    * **Cooldown:** There is a fixed **0.5-second cooldown** period between consecutive shots.
* **Enemies:**
    * **Red Drones (🟥):** Fire random **green projectiles** that deal **1 damage** to the player.
    * **Blue Drones (Megatrons) (🟦):** Fire **homing orange projectiles** that deal **3 damage** to the player.
    * **Tanks (⬜):** Launch **purple shells** that deal **5 damage** to the player.
* **Points:**
    * Destroying a **Red Drone:** +10 points
    * Destroying a **Megatron:** +100 points
    * Destroying a **Tank:** +50 points

### Health & Power-Ups
* **Health:** The player's survival begins with **100 Health Points**. The game concludes if the player's health reaches 0.
* **Medboxes (❌):** Collecting a medbox instantly restores **25 Health Points**.
* **Shields (🔵):** Upon collection, a shield grants the player **5 seconds of complete invincibility**.

### Enemy Behavior
* **Red Drones:** Exhibit random flight patterns within the arena. They spawn every **5 seconds**, concurrently with tanks.
* **Megatrons:** Actively track the player's movement and fire homing projectiles. They spawn every **10 seconds**.
* **Tanks:** Navigate along the ground surface of the arena. Their turrets continuously aim at the player's position. They spawn every **5 seconds**, concurrently with red drones.

### Power-Up Spawning
* **Shields (🔵):** Spawn randomly within the arena every **10 seconds**.
* **Medboxes (❌):** Spawn randomly within the arena every **10 seconds**.

## Controls

* **V:** Toggles the camera perspective between **first-person** and **third-person view**.
* **P:** **Pauses** or **resumes** the current game state.
* **R:** **Restarts** the game. This function is only active and usable when the game is paused.
* **Q** / **Esc:** **Quits** the game application entirely.

## HUD Elements

The Heads-Up Display provides crucial information during gameplay:
* **Health Bar (Top-Left):** Visually represents the player's current health.
* **Shield Timer (Cyan, Below Health):** Indicates the remaining duration of the invincibility shield when active.
* **Score (Top-Right):** Displays the player's current accumulated score.
* **Kills (Top-Right):** Shows the total number of enemies the player has defeated.
* **Time Survived (Top-Right):** Tracks the total time the player has managed to stay alive (excluding any paused time).
* **Gun Level (Top-Right):** Indicates the current damage level of the player's weapon.
* **"GAME OVER" Screen:** Appears when the player's health reaches zero, pausing the game.

## Advanced Features

### Gun Progression
The damage of the player's bullets scales dynamically with their score, increasing by **1 damage point for every 100 points** earned.

### Bullet Types
* **Player:** Fires **yellow bullets** whose damage is determined by the current gun level.
* **Enemies:** Utilize distinct color-coded projectiles for easy identification: **green** (Red Drones), **orange** (Megatrons), and **purple** (Tanks).

### Pause Mechanics
When the game is paused, all gameplay elements are frozen, and the survival timer is temporarily stopped.

## Game Over & Restart

### Loss Condition
The game ends when the player's **health is depleted to 0**.

### Restart
While the game is **paused**, pressing the **`R` key** will initiate a restart. This action resets the player's health, score, kill counts, and survival time, allowing for a new game session.


