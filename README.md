# Saber Siege

A top-down arena survival game: swing a lightsaber through endless waves of zombies.

Built with plain HTML5 canvas and vanilla JavaScript, with no build step. The classic top-down mode has no dependencies; the first-person mode uses a bundled copy of Three.js.

## Play

Open `index.html` in any modern browser, or serve the folder:

```
npx serve .
```

## Controls

| Input | Action |
| --- | --- |
| WASD / Arrow keys | Move |
| Mouse | Aim the saber |
| Left click | Swing |
| Right click / Space | Force push (knocks back and stuns nearby zombies) |
| Shift | Dash |
| P / Esc | Pause |
| M | Toggle mouse-follow movement |

**Mouse-follow mode** (toggle with `M` or the button on the title screen; the choice is remembered): the player walks toward the cursor, faster the farther it is, and stops when the cursor is close. WASD still overrides it while held, and Dash goes toward the cursor.

## First-person mode

`fps.html` is a 3D first-person version of the same game (there is a link to it on the title screen, and a link back).
It uses [Three.js](https://threejs.org) r149, bundled in `vendor/` so it still works offline and when opened as a file.

| Input | Action |
| --- | --- |
| WASD / Arrow keys | Move |
| Mouse | Look around (the pointer is captured while playing) |
| Left click | Swing: the blade cuts whatever is in reach in front of you |
| Right click / Space | Force push |
| Shift | Dash |
| P / Esc | Pause |

The radar at the top shows zombies around you, and a red arc shows where a hit came from. You regain a little health at the start of each wave.
On a phone: left thumb moves, right thumb drags to look, and the saber swings by itself when a zombie is in reach. If you are not dragging to look, the view turns toward the nearest zombie.

## Playing on iPhone / iPad

The game has a touch mode that switches on automatically when you touch the screen:

- Drag anywhere on the left side to move (floating joystick)
- The saber auto-aims at the nearest zombie and swings when one is in range
- Buttons on the right: **Swing**, **Force**, **Dash**; the pause button is at the top

To install it like an app, host the folder over HTTPS (GitHub Pages works: Settings → Pages → deploy from the branch root),
open the URL in Safari, tap **Share → Add to Home Screen**, and launch it from the icon. It runs fullscreen and works offline.
Landscape orientation is recommended.

## Features

- Six saber colors to choose from
- Four zombie types: walkers, fast runners, armored brutes, and spitters whose projectiles you can deflect with the blade
- Escalating waves, combo multiplier, screen shake, particle effects, and synthesized sound (no audio files)
