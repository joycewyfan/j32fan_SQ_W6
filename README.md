# Side Quest Week 6

## Setup and Interaction Instructions

To run the sketch locally, open `index.html` in Google Chrome using Live Server.

**Controls:**
- Move: WASD
- Shoot: Spacebar (shoots in the direction you last moved)
- B: Skip to boss fight (testing only)
- Restart: R (after win or game over)

Explore the world, survive enemy waves as you move north, then enter the glowing boss zone to fight the giant orange blob. Watch the minimap to track enemies off screen.

**Adding Your Own Sounds**
1. Add your sound files to `assets/sounds/`
2. In `preload()`, uncomment the `loadSound()` lines and update the file paths
3. Uncomment the `play()` or `loop()` calls in the relevant functions — there are hooks for the boss music transition too

**Editing the Waves and Boss**
Open `data/enemies.json` to change when waves spawn, how many enemies appear, their speed, and the boss stats. Each wave has a `spawnAt` world Y value — lower values trigger later since the player starts at the bottom of the world.

**Opening the Chrome Console**
- **Windows:** Press `F12` or `Ctrl + Shift + J`, then click the **Console** tab
- **Mac:** Press `Cmd + Option + J`

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

