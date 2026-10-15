# APSU Lockpicking Prototype

A standalone browser lockpicking minigame developed as a feature prototype for [APSU Roleplay](https://github.com/pbrizendine/apsu), a browser-based roleplaying platform.

This repository preserves the original single-file prototype, rather than the later integrated APSU implementation. HTML, CSS, and JavaScript are contained in `index.html`. No installation, account is required. 

## Play locally

Download the repository and open `index.html` in a modern browser.

1. Choose Easy, Moderate, or Hard.
2. Drag the pick from the corner into the keyhole.
3. Hold Q/E or the on-screen left/right controls to adjust the pick.
4. Hold Space or Try Lock to attempt the lock. Incorrect angles damage the pick; attempts are limited.
5. Complete three stages to open the lock. Select a difficulty to restart.

* Pointer interaction also supports dragging and manipulating the pick. Keyboard controls become active after insertion.

## How it works

- A randomly selected target angle defines the successful range.
- Difficulty controls angle tolerance, attempt limits, and damage rate.
- A `requestAnimationFrame` loop updates movement, progress, damage, and visual feedback using elapsed time.
- Pointer and keyboard events update input state.
- The game tracks insertion, attempts, pick health, stage progress, and success/failure.

## Relationship to APSU

This is one APSU gameplay feature, shared separately so it can be played and studied without the full multiplayer experience. The prototype is provided for demonstration and continued development. Some aspects are outdated and may need refinement. 
