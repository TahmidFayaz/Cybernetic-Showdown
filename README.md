# -Cybernetic-Showdown

Objective
Survive as long as possible by shooting enemies while avoiding their attacks. Collect power-ups to boost your chances. Achieve a high score by killing enemies and surviving.

Core Mechanics
Movement
WASD Keys: Move forward (W), left (A), backward (S), right (D).
Bounding: Player is confined to an arena (-50 to +50 on X/Z axes).

Combat
Shooting:
Left mouse click or Spacebar to fire.
0.5-second cooldown between shots.
Bullets travel straight in the direction the player is aiming.

Enemies:
Small Drones (Red): 1 HP, 10 points.
Megatrons (Blue): 3 HP, 100 points.
Tanks (Grey): 5 HP, 50 points. Shoot purple projectiles at the player.

Health & Power-Ups
Health: Starts at 100. Game over at 0.
Medboxes (Red cubes with white crosses): Restore 25 HP when collected.
Shields (Cyan spheres): Grant 5 seconds of invincibility when collected.

Enemy Behavior
Drones: Fly randomly within the arena, bouncing off boundaries.
Tanks:
Move on the ground and fire projectiles every 3–7 seconds.
Turrets track the player’s position.

Spawning:
New enemies spawn every 5 seconds (max 10 total).
Higher chance for small drones than other entities.

Controls
V: Toggle between first-person and third-person views.
P: Pause/resume the game.
R: Restart the game (after death or during play).
Q/Esc: Quit the game.

Mouse: Look around (mouse movement controls camera aim).

Scoring & Progression
Points:
Small drone: +10
Tank: +50
Megatron: +100

Stats Tracked:
Total score.
Tanks/Megatrons killed.
Time survived (in seconds).

Game Over & Restart
Loss Condition: Player health reaches 0.
Game Over Screen: Displays "GAME OVER" and pauses gameplay.
Restart: Press R to reset all stats and entities.
