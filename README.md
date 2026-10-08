# Saber Siege

A top-down arena survival game: swing a lightsaber through endless waves of zombies.

Built with plain HTML5 canvas and vanilla JavaScript — no build step, no dependencies.

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
