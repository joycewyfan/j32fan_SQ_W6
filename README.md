# Side Quest Week 6

## Setup and Interaction Instructions

To run the sketch locally, open `index.html` in Google Chrome using Live Server.

**Controls:**
- Move: WASD
- Shoot: Spacebar (shoots in the direction you last moved)
- B: Skip to boss fight (testing only)
- Restart: R (after win or game over)

You begin near the bottom of a large world and must travel north while surviving enemy waves. As you progress, enemy groups will spawn based on your position in the world. Avoid obstacles, manage your health, and defeat enemies to increase your score.

When you reach the glowing boss zone near the top of the map, a giant orange blob boss will appear. Defeat the boss to win the game.

The minimap in the bottom-left corner displays:
- Your current position (teal)
- Enemy locations (orange)
- Boss location (red)
- The current camera view
- The boss zone area

**Adding Your Own Sounds**
The game uses audio files loaded in preload(). To replace or add sounds:

1. Place your sound files inside the assets/sounds/ folder.
2. Update the corresponding loadSound() file paths in the preload() function.
3. Modify or uncomment the appropriate play() or loop() calls within the game logic to trigger the new sounds.

Separate audio hooks are included for shooting, player damage, boss damage, background music, boss music, and victory sounds, allowing easy customization.

**Editing the Waves and Boss**
The file data/enemies.json stores all enemy wave and boss configuration data.
Enemy Waves

Each wave contains:
- spawnAt – the player's world Y-coordinate that triggers the wave
- enemies – a list of enemies and their movement speeds

Increasing the number of enemy objects or their speed values will increase the game's difficulty. Since the player starts near the bottom of the world and moves upward, lower spawnAt values cause waves to appear later in the game.
Boss Settings

The boss object controls the boss battle and can be customized by changing:
- health
- radius (r)
- chargeSpeed
- retreatSpeed
- chargePause
- retreatY

These values allow the boss's difficulty and behaviour to be adjusted without modifying the main game code.

Obstacle positions are stored in data/obstacles.json.

Each obstacle contains:
- x – horizontal position in the world
- y – vertical position in the world
- size – the dimensions of the obstacle

You can easily redesign the map by adding, removing, or repositioning obstacles 
within this file without changing the collision or rendering code.

## Assets

| File | Source |
|---|---|
| `assets/images/background.png` | Created with Copilot |
| `assets/sounds/bossHit.mp3` [1]| pixabay.com |
| `assets/sounds/bossMusic.mp3` [2]| pixabay.com |
| `assets/sounds/darkforest.mp3`[3]| pixabay.com |
| `assets/sounds/hit.mp3` [4]| pixabay.com |
| `assets/sounds/PlayerHit.mp3` [5]| pixabay.com |
| `assets/sounds/shoot.mp3` [6]| pixabay.com |
| `assets/sounds/victory.mp3` [7]| pixabay.com | 

## References

[1] https://pixabay.com/sound-effects/film-special-effects-punch-knuckle-blunt-medium-503895/ Pixabay. Sound effect used for punch sound effect. Retrieved June 17, 2026, from https://pixabay.com/sound-effects/film-special-effects-punch-knuckle-blunt-medium-503895/

[2] https://pixabay.com/sound-effects/musical-cinematic-action-epic-trailer-inception-part-1-short-preview-488564/ Pixabay. Background music used during gameplay. Retrieved June 17, 2026, from https://pixabay.com/sound-effects/musical-cinematic-action-epic-trailer-inception-part-1-short-preview-488564/

[3] https://pixabay.com/sound-effects/nature-forest-soundscape-night-time-403609/ Pixabay. Ambient forest soundscape used for background audio. Retrieved June 17, 2026, from https://pixabay.com/sound-effects/nature-forest-soundscape-night-time-403609/

[4] https://pixabay.com/sound-effects/film-special-effects-jump-sound-531048/ Pixabay. Sound effect used for jump action. Retrieved June 17, 2026, from https://pixabay.com/sound-effects/film-special-effects-jump-sound-531048/

[5] https://pixabay.com/sound-effects/film-special-effects-hit-by-a-wood-230542/ Pixabay. Sound effect used for hit or collision events. Retrieved June 17, 2026, from https://pixabay.com/sound-effects/film-special-effects-hit-by-a-wood-230542/

[6] https://pixabay.com/sound-effects/film-special-effects-swoosh-sound-effect-for-fight-scenes-or-transitions-2-149890/ Pixabay. Swoosh sound effect used for attack or transition animations. Retrieved June 17, 2026, from https://pixabay.com/sound-effects/film-special-effects-swoosh-sound-effect-for-fight-scenes-or-transitions-2-149890/

[7] https://pixabay.com/sound-effects/film-special-effects-11l-victory-beat-1749704521130-358766/ Pixabay. Sound effect used for victory screen. Retrieved June 17, 2026, from https://pixabay.com/sound-effects/film-special-effects-11l-victory-beat-1749704521130-358766/

