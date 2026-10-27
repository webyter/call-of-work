# Call of Work

A single-page 3D FPS built with HTML, CSS, JavaScript, and Three.js. The current playable build includes bot matches, multiple maps and match modes, weapon loadouts, attachments, touch controls, and session-based progression.

## Run locally

Serve this directory using a static web server:

```sh
python3 -m http.server 8000
```

Open http://localhost:8000 in a modern browser with WebGL support. An internet connection is required to load Three.js and other external resources.

## Play

Select a map, match mode, and bot difficulty, then press **DEPLOY**.

| Action | Desktop control |
| --- | --- |
| Move | WASD |
| Look | Mouse |
| Fire / aim | Left / right mouse button |
| Sprint | Shift |
| Jump | Space |
| Crouch / slide | C |
| Reload | R |
| Switch weapons | 1 / 2 or mouse wheel |
| Tactical / frag grenade | Q / G |
| Scorestreaks | 3 / 4 / 5 |
| Pause | Escape |

Touch devices use on-screen controls. Landscape orientation is recommended.

## Features

- Team Deathmatch, Domination, Kill Confirmed, and Free-for-All.
- Killhouse, Freight Yard, and Blacksite maps.
- Teammates and enemy bots.
- Assault rifle, SMG, shotgun, and sniper loadouts.
- Weapon attachments, character customization, and weapon skins.
- XP, ranks, and camo challenges.
- Killer-view camera replay.
- Customizable phone controls and aiming settings.

## Current limitations

- This is a local bot game, not an online multiplayer service.
- The embedded-preview build uses fallback mouse controls instead of pointer capture.
- Progress is held in memory for the current page session. Refreshing resets it.
- The killer-view replay replays camera motion while the world continues live; it is not a full-world replay.
- Real-device phone performance has not been benchmarked.

## Project structure

`index.html` contains the interface, styles, and game logic. No build step or backend is required.
